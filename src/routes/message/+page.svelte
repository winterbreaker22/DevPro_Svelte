<script>
  import { Button, ButtonGroup } from "flowbite-svelte";
</script>

<div class="mx-32 my-20">
  <h1 class="text-left mb-4">CHATS</h1>
  <div class="flex bg-primary-4 rounded-2xl">
    <div class="w-1/4 min-h-[1300px] m-3">
      <!-- address -->
      <div class="bg-primary-0 rounded-2xl mb-3 min-h-[900px] px-4 py-3 flex flex-col">
        <div class="flex text-center border border-1 text-white border-primary-1 p-[2px] rounded-2xl">
          <div class="w-1/2 bg-primary-1 py-2 rounded-l-2xl">MAIN</div>
          <div class="w-1/2 py-2">GROUPS</div>
        </div>
      </div>
      <!-- detail -->
      <div class="bg-primary-0 rounded-2xl min-h-[388px]"></div>
    </div>

    <!-- chat board -->
    <div class="w-1/2 min-h-[1300px] bg-primary-0 rounded-2xl my-3"></div>

    <div class="w-1/4 min-h-[1300px] m-3">
      <!-- order -->
      <div class="bg-primary-0 rounded-2xl mb-3 min-h-[650px]"></div>
      <!-- suggestion -->
      <div class="bg-primary-0 rounded-2xl min-h-[638px]"></div>
    </div>
  </div>
</div>

<style>
</style>
