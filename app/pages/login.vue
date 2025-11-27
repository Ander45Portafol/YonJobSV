<template>
  <div class="w-full h-screen flex flex-row bg-[#051E51]">
    <!--PARTE IZQUIERDA: Formulario-->
    <div
      class="w-full md:w-1/2 bg-[#021B4A] flex flex-col justify-center px-6 md:px-20"
    >
      <div class="mb-5">
        <img src="/YonJobIcon.png" alt="" srcset="" />
      </div>
      <h3 class="text-white font-bold text-2xl mb-2">
        Inicia sesión con tu cuenta
      </h3>
      <p class="text-white mb-5">
        ¿No tienes cuenta?
        <a class="text-[#5A91FF] font-semibold cursor-pointer">Regístrate</a>
      </p>
      <!--Inicio del formulario de Login-->
      <form>
        <div class="space-y-12">
          <div class="mt-6 grid grid-cols-1 gap-x-6 gap-y-8 sm:grid-cols-6">
            <div class="sm:col-span-6">
              <div>
                <label
                  for="email"
                  class="block text-sm/6 font-medium text-white"
                  >Correo electrónico</label
                >
                <div class="mt-2">
                  <input
                    id="email"
                    type="email"
                    name="email"
                    placeholder=""
                    class="block w-full rounded-md bg-white/5 px-3 py-1.5 text-base text-white outline-1 -outline-offset-1 outline-white/10 placeholder:text-gray-500 focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-500 sm:text-sm/6 h-10"
                  />
                </div>
              </div>
            </div>
            <div class="sm:col-span-6">
              <div>
                <label
                  for="email"
                  class="block text-sm/6 font-medium text-white"
                  >Contraseña</label
                >
                <div class="mt-2">
                  <input
                    id="email"
                    type="email"
                    name="email"
                    placeholder=""
                    class="block w-full rounded-md bg-white/5 px-3 py-1.5 text-base text-white outline-1 -outline-offset-1 outline-white/10 placeholder:text-gray-500 focus:outline-2 focus:-outline-offset-2 focus:outline-indigo-500 sm:text-sm/6 h-10"
                  />
                </div>
              </div>
            </div>
          </div>
        </div>
      </form>
      <!-- Forgot password -->
      <a
        class="text-[#78EF97] font-semibold text-sm mt-2 mb-5 cursor-pointer self-end"
      >
        ¿Olvidaste tu contraseña?
      </a>
      <!-- Botón login -->

      <NuxtLink to="/dashboard">
        <button
          class="w-full h-12 bg-[#78EF97] text-white font-semibold rounded-lg mt-2"
        >
          Iniciar sesión
        </button>
      </NuxtLink>

      <!-- Línea separadora -->
      <div class="flex items-center my-6">
        <span class="flex-1 h-px bg-white"></span>
        <span class="px-4 text-white text-sm">O continúa con</span>
        <span class="flex-1 h-px bg-white"></span>
      </div>
      <!-- Google -->
      <button
        class="w-full h-12 bg-white text-[#5A91FF] font-bold rounded-lg flex items-center justify-center gap-2"
      >
        <img src="/googleIcon.svg" class="w-5" /> Google
      </button>
    </div>

    <!--Inicio imagen de Derecha-->
    <div class="w-1/2 relative hidden md:block">
      <img class="w-full h-full object-cover" src="/M_programming.png" />
    </div>
  </div>
</template>
