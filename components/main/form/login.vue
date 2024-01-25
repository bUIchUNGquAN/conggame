<template>
  <div
    v-if="visible"
    class="fixed top-0 left-0 w-full h-full flex justify-center items-center bg-black bg-opacity-50"
  >
    <div class="bg-white p-8 rounded-md">
      <h2 class="text-2xl font-bold mb-4">Login Form</h2>

      <UFormGroup label="Username">
        <UInput v-model="username" placeholder="Enter your username" />
      </UFormGroup>
      <UFormGroup label="Password">
        <UInput
          v-model="password"
          type="password"
          placeholder="Enter your password"
        />
      </UFormGroup>
      <div class="mt-4">
        <UButton @click="handleLogin">Login</UButton>
      </div>
    </div>
  </div>
</template>

<script setup>
const visible = ref(false);
const username = ref("");
const password = ref("");

const handleLogin = () => {
  console.log("Logging in with:", username.value, password.value);

  visible.value = false;
};
</script>
