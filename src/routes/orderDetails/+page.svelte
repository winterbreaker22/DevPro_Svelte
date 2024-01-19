  
  <script>
    import { Listgroup, ListgroupItem, Button } from 'flowbite-svelte';

    const orderDetails = [
      {
        title: "Product title",
        content: "Banana 3D Model"
      },
      {
        title: "Product description",
        content: "A 3D model of a yellow banana with textures and a UV Map"
      },
      {
        title: "Order number",
        content: "2673901020"
      },
      {
        title: "Program",
        content: "Blender"
      },
      {
        title: "Start date",
        content: "February 23, 1978"
      },
      {
        title: "Expected delivery",
        content: "April 2, 2079"
      },
      {
        title: "Total price",
        content: "$923.22"
      },
      {
        title: "Need help?",
        content: "Click Here"
      }
    ]
  </script>
  
  <Listgroup active class="w-48">
    <h3 class="p-1 text-center text-xl font-medium text-gray-900 dark:text-white">Suggestions</h3>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">{orderDetails[0].title}</h5>
      <p>{orderDetails[0].content}</p>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">{orderDetails[1].title}</h5>
      <p>{orderDetails[1].content}</p>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">{orderDetails[2].title}</h5>
      <p>{orderDetails[2].content}</p>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">{orderDetails[3].title}</h5>
      <p>{orderDetails[3].content}</p>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">{orderDetails[4].title}</h5>
      <p>{orderDetails[4].content}</p>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">{orderDetails[5].title}</h5>
      <p>{orderDetails[5].content}</p>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">{orderDetails[6].title}</h5>
      <p>{orderDetails[6].content}</p>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">{orderDetails[7].title}</h5>
      <p>{orderDetails[7].content}</p>
    </ListgroupItem>
    <a href="/" class="flex items-center p-3 text-sm font-medium text-red-600 bg-gray-50 hover:bg-gray-100 dark:bg-gray-700 dark:hover:bg-gray-600 dark:text-red-500 hover:underline rounded-b-lg">
      ORDER AGAIN
    </a>
  </Listgroup>
