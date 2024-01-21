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
  import directCurious from "$lib/images/Ellipse 31.png";
  import phonesolid from "$lib/images/phone-solid 1.svg";
  import videosolid from "$lib/images/video-solid 1.svg";
  import groupsolid from "$lib/images/Group 74.svg";
  import paperclip from "$lib/images/paperclip-solid 1.png";
  import microphone from "$lib/images/microphone-solid 1.png";
  import facegrin from "$lib/images/face-grin-stars-solid 1.png";
  import chevronRight from "$lib/images/chevron-right-solid 2.png";
  import { ChevronDownSolid } from 'flowbite-svelte-icons';
  import { Dropdown, DropdownItem, DropdownDivider } from 'flowbite-svelte';

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

<style>
  .chat-segment span {
    font-size: 20px; color: white;
    padding: 12px;
  } 
  .chat-send .chat-segment {
    padding: 12px 4px 0px 14px;
  }
  .chat-send .chat-segment span {
    display: inline-flex;
    float: right;
    justify-content: flex-end;
    align-items: center;
    border-radius: 12px 0px 12px 12px;
    background: #FF8A00;
  }
  .chat-receive .chat-segment {
    padding: 11px 11px 0px 5px;
  }
  .chat-receive .chat-segment span {
    display: inline-flex;
    float: left;
    align-items: center;  
    border-radius: 12px 0px 12px 12px;
    background: #373737;
  }
  #chatting, #chatting > div{
    display: flex; flex-direction: column-reverse; justify-content: flex-start; padding-bottom: 20px;
  }
</style>

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
    <div class="w-1/2 min-h-[1300px] bg-primary-0 rounded-2xl my-3" style="padding: 13px 26px;">
      <div class="direct-curious" style="display: flex; justify-content: space-between;">
        <div style="display: flex; height: 76px;">
          <img src={directCurious} alt="direct" style="margin-right: 11px;">
          <div>
            <h4 style="color: #FF8A00; font-size: 25px;">curiousgeorge</h4>
            <p style="color: #FF8A00; font-size: 10px;">Last active 2 minutes ago</p>
          </div>
        </div>
        <div style="padding: 13px 26px; display: flex; align-items: center; gap: 22px;">
          <img src={phonesolid} alt="phone" >
          <img src={videosolid} alt="video" >
          <div><img src={groupsolid} alt="group" style="margin-top: 10px;"><ChevronDownSolid class="w-3 h-3 ms-2 text-primary-0 dark:text-white" /></div>
          <Dropdown >
            <DropdownItem class="font-bold">SHARE PROFILE</DropdownItem>
            <DropdownItem class="font-bold">REPORT</DropdownItem>
            <DropdownItem class="text-primary-6 font-bold">BLOCK USER</DropdownItem>
          </Dropdown>
        </div>
      </div>
      <div class="chat-part" style="display: flex; flex-direction: column-reverse; justify-content: flex-start; height: calc(100% - 76px); padding-bottom: 20px;">
        <form id="chat-input" style="display: flex; justify-content: space-between; gap: 8px;">
          <div style="width: 100%; display: inline-flex; padding-top: 2px; padding-bottom: 2px; padding-left: 14px; align-items: center; border-radius: 12px; background: #D9D9D9; justify-content: space-between;">
            <input type="text" style="background: #D9D9D9; color: #BABABA; font-size: 20px; font-style: normal; font-weight: 400; line-height: 111%; letter-spacing: -0.2px; border: none;" placeholder="Type here...">
            <div style="display: flex;">
              <img src={facegrin} alt="face" style="padding-right: 10px;">
              <img src={microphone} alt="microphone" style="padding-right: 10px;">
              <img src={paperclip} alt="papaer" style="padding-right: 10px;">
            </div>
          </div>
          <input type="submit" value=">" style="color: white; width: 64px; height: 42px; flex-shrink: 0; border-radius: 10px; background: #FF8A00; font-size: 17px;">
        </form>
        <div style="padding-top: 27px; padding-bottom: 27px;">
          <svg xmlns="http://www.w3.org/2000/svg" width="69" height="21" viewBox="0 0 69 21" fill="none">
            <circle cx="10.0161" cy="10.0161" r="10.0161" fill="white"/>
            <circle cx="34.4995" cy="10.0161" r="10.0161" fill="white" fill-opacity="0.5"/>
            <circle cx="58.9839" cy="10.0161" r="10.0161" fill="white" fill-opacity="0.5"/>
          </svg>
        </div>
        <div id="chatting">
          <div class="chat-send"> 
            <div class="chat-segment"><span>I found your papers!</span></div>
            <div class="chat-segment"><span>Hey</span></div>
          </div>
          <div class="chat-receive"> 
            <div class="chat-segment"><span>do you have my papers?</span></div>
          </div>
        </div>
        <p class="text-center" style="margin-bottom: 27px; color: rgba(255, 255, 255, 0.70); font-size: 10px; font-weight: 400; line-height: normal; letter-spacing: -0.1px;">SATURDAY - MARCH 6, 2021 AT 4:59PM</p>
      </div>
    </div>

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
