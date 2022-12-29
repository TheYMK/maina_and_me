<script>
  // your script goes here

  import Navbar from "../../components/Navbar.svelte";
  let currentStep = 1;
</script>

<Navbar />
{#if currentStep === 1}
  <div
    class="h-screen flex flex-col justify-center items-center text-center p-10 lg:p-72"
  >
    <p>
      I always wondered if true love existed, but then I found you, and I found
      answers to all my questions. It was so easy to love you, to pamper you, to
      be there with you. <br /><br /> Thank you for teaching me to love and be loved
      and make this life a fairytale. I wish we always stay together and celebrate
      our relationship with the same energies and sparkles as we do today.
    </p>
    <button
      class="btn btn-neutral self-center mt-10"
      on:click={() => (currentStep = 2)}>Continue</button
    >
  </div>
{:else if currentStep === 2}
  <div
    class="h-screen flex flex-col justify-center items-center text-center p-10 lg:p-72"
  >
    <img src="/mom.jpg" alt="" class="w-72" />
    <p class="font-bold text-3xl mt-10">Do you remember this day ?</p>
    <div class="flex flex-row gap-2">
      <button
        class="btn btn-neutral self-center mt-10"
        on:click={() => (currentStep = 3)}>Yes</button
      >
      <button
        class="btn btn-error self-center mt-10"
        on:click={() => (currentStep = 0)}>No</button
      >
    </div>
  </div>
{:else if currentStep === 3}
  <div
    class="h-screen flex flex-col justify-center items-center text-center p-10 lg:p-72"
  >
    <p class="font-bold text-3xl mt-10">
      Well I think it's about time we renew our vows
    </p>
    <button
      class="btn btn-neutral self-center mt-10"
      on:click={() => (currentStep = 4)}>Continue</button
    >
  </div>
{:else if currentStep === 4}
  <div
    class="h-screen flex flex-col justify-center items-center text-center p-10 lg:p-72"
  >
    <p class="font-bold text-3xl mt-10">Do you still love me ?</p>
    <div class="flex flex-row gap-2">
      <button
        class="btn btn-neutral self-center mt-10"
        on:click={() => (currentStep = 5)}>Yes</button
      >
      <button
        class="btn btn-error self-center mt-10"
        on:click={() => (currentStep = 0)}>No</button
      >
    </div>
  </div>
{:else if currentStep === 5}
  <div
    class="h-screen flex flex-col justify-center items-center text-center p-10 lg:p-72"
  >
    <p class="font-bold text-3xl mt-10">
      Do you still want to spend the rest of your life with me ?
    </p>
    <div class="flex flex-row gap-2">
      <button
        class="btn btn-neutral self-center mt-10"
        on:click={() => (currentStep = 6)}>Yes</button
      >
      <button
        class="btn btn-error self-center mt-10"
        on:click={() => (currentStep = 0)}>No</button
      >
    </div>
  </div>
{:else if currentStep === 6}
  <div
    class="h-screen flex flex-col justify-center items-center text-center p-10 lg:p-72"
  >
    <p class="font-bold text-3xl mt-10">Sure .... ?</p>
    <div class="flex flex-row gap-2">
      <button
        class="btn btn-neutral self-center mt-10"
        on:click={() => (currentStep = 7)}>Yes</button
      >
      <button
        class="btn btn-error self-center mt-10"
        on:click={() => (currentStep = 0)}>No</button
      >
    </div>
  </div>
{:else if currentStep === 7}
  <div
    class="h-screen flex flex-col justify-center items-center text-center p-10 lg:p-72"
  >
    <p class="font-bold text-3xl mt-10">Okayyyyy giiirl if you say sooooo...</p>
    <div>
      <button
        class="btn btn-neutral self-center mt-10"
        on:click={() => (currentStep = 8)}>Continue</button
      >
    </div>
  </div>
{:else if currentStep === 8}
  <div
    class="h-screen flex flex-col justify-center items-center text-center p-10 lg:p-72"
  >
    <img src="/ring.png" alt="" class="w-72" />

    <p class="font-bold text-3xl mt-10">
      Will you be my fiancé until we get my married ?
    </p>
    <div class="flex flex-row gap-2">
      <button
        class="btn btn-neutral self-center mt-10"
        on:click={() => (currentStep = 9)}>Yes</button
      >
      <button
        class="btn btn-error self-center mt-10"
        on:click={() => (currentStep = 0)}>No</button
      >
    </div>
  </div>
{:else if currentStep === 9}
  <div
    class="h-screen flex flex-col justify-center items-center text-center p-10 lg:p-72"
  >
    <img src="/ring.png" alt="" class="w-72" />

    <p class="font-bold text-3xl mt-10">
      Thank you...I promise to love you more than you could ever imagine
    </p>
    <button
      class="btn btn-neutral self-center mt-10"
      on:click={() => (window.location.href = "/")}>This is the end</button
    >
  </div>
{/if}

<style>
  /* your styles go here */
</style>
