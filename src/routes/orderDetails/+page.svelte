  
  <script>
    import { Listgroup, ListgroupItem, Button } from 'flowbite-svelte';
    import { TrashBinSolid } from 'flowbite-svelte-icons';
  </script>
  
  <Listgroup active class="w-48">
    <h3 class="p-1 text-center text-xl font-medium text-gray-900 dark:text-white">Suggestions</h3>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">Product title</h5>
      <p>Banana 3D Model</p>
      <Button>Add</Button>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">Product description</h5>
      <p>A 3D model of a yellow banana with textures and a UV Map</p>
      <Button>Add</Button>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">Order number</h5>
      <p>2673901020</p>
      <Button>Add</Button>
    </ListgroupItem>
    <a href="/" class="flex items-center p-3 text-sm font-medium text-red-600 bg-gray-50 hover:bg-gray-100 dark:bg-gray-700 dark:hover:bg-gray-600 dark:text-red-500 hover:underline rounded-b-lg">
      <TrashBinSolid class="w-6 h-6 ms-1 me-2" />
      ORDER AGAIN
    </a>
  </Listgroup>
