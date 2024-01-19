<script>
  import { Button, ButtonGroup, Search } from "flowbite-svelte";
  import avatar1 from "$lib/images/img1.jpg";
  import avatar2 from "$lib/images/Group 63.png";
  import avatar3 from "$lib/images/Rectangle 47.png";
  import avatar4 from "$lib/images/Rectangle 94.png";
  import avatar5 from "$lib/images/Rectangle 97.png";
  import avatar6 from "$lib/images/Rectangle 98.png";
  import avatar7 from "$lib/images/Rectangle 99.png";
  import downArrow from "$lib/images/Vector.svg";
 
  import { Button, ButtonGroup } from "flowbite-svelte";
  import Suggestions from "../suggestions/+page.svelte";
  import OrderDetails from "../orderdetails/+page.svelte";
  import CuriousGeorge from "../curiousGeorge/+page.svelte";
  
  let items = [
    {
      avatar: avatar1,
      name: "curiousgeorge",
      lastMessage: "",
    },
    {
      avatar: avatar2,
      name: "maxvers",
      lastMessage: "yo. whats up",
    },
    {
      avatar: avatar3,
      name: "timothee_chal",
      lastMessage: "yo. whats up",
    },
    {
      avatar: avatar4,
      name: "porsheusa",
      lastMessage: "yo. whats up",
    },
    {
      avatar: avatar5,
      name: "charlesleclerc",
      lastMessage: "yo. whats up",
    },
    {
      avatar: avatar6,
      name: "goerge.russell",
      lastMessage: "yo. whats up",
    },
    {
      avatar: avatar7,
      name: "lewishamilton",
      lastMessage: "yo. whats up",
    },
    {
      avatar: avatar1,
      name: "curiousgeorge",
      lastMessage: "",
    },
    {
      avatar: avatar2,
      name: "maxvers",
      lastMessage: "yo. whats up",
    },
    {
      avatar: avatar3,
      name: "timothee_chal",
      lastMessage: "yo. whats up",
    },
    {
      avatar: avatar4,
      name: "porsheusa",
      lastMessage: "yo. whats up",
    },
  ];
</script>

<svelte:head>
  <title>Message</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>

<div class="mx-32 my-20">
  <h1 class="text-left mb-4">CHATS</h1>
  <div class="flex bg-primary-4 rounded-2xl">
    <div class="w-1/4 min-h-[1300px] m-3">
      <!-- address -->
      <div
        class="bg-primary-0 rounded-2xl mb-3 min-h-[900px] px-4 py-3 flex flex-col cursor-pointer"
      >
        <div
          class="flex text-center border border-1 text-white border-primary-1 p-[2px] rounded-2xl mb-[14px]"
        >
          <div class="w-1/2 bg-primary-1 py-2 rounded-l-2xl">MAIN</div>
          <div class="w-1/2 py-2">GROUPS</div>
        </div>

        <Search size="sm" class="rounded-2xl" placeholder=""></Search>

        <div>
          {#each items as item, index}
            <div
              class="border-2  py-2 px-4 bg-opacity-25 my-[14px] rounded-xl flex items-center h-[51px] {index == 0 ? 'bg-primary-1 border-primary-1' : 'border-primary-4 text-primary-4'}"
            >
              <img
                src={item.avatar}
                alt=""
                class="w-[35px] h-[35px] rounded-full mr-2"
              />
              {#if item.lastMessage}
                <div>
                  <p>{item.name}</p>
                  <p class="reading-[13px] text-[13px]">{item.lastMessage}</p>
                </div>
              {:else}
                {item.name}
              {/if}
            </div>
          {/each}
          <div class="flex justify-center mt-8">
            <img src={downArrow} alt="" >
          </div>
        </div>
      </div>
      <!-- detail -->
      <div class="bg-primary-0 rounded-2xl min-h-[388px]">
        <CuriousGeorge />
      </div>
    </div>

    <!-- chat board -->
    <div class="w-1/2 min-h-[1300px] bg-primary-0 rounded-2xl my-3"></div>

    <div class="w-1/4 min-h-[1300px] m-3">
      <!-- order -->
      <div class="bg-primary-0 rounded-2xl mb-3 min-h-[650px]">
        <OrderDetails />
      </div>
      <!-- suggestion -->
      <div class="bg-primary-0 rounded-2xl min-h-[638px]">
        <Suggestions />
      </div>
    </div>
  </div>
</div>

<style>
</style>
