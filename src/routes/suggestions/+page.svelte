  
  <script>
    import { Listgroup, ListgroupItem, Avatar, Button } from 'flowbite-svelte';
    import { TrashBinSolid } from 'flowbite-svelte-icons';
  </script>
  
  <Listgroup active class="w-48">
    <h3 class="p-1 text-center text-xl font-medium text-gray-900 dark:text-white">Suggestions</h3>
    <ListgroupItem class="text-base font-semibold gap-2">
      <Avatar src="/images/suggestions/Ellipse 30 (1).png" size="xs" />Jese Leos
      <Button>Add</Button>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <Avatar src="/images/suggestions/Ellipse 30 (2).png" size="xs" />Robert Gouth
      <Button>Add</Button>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <Avatar src="/images/suggestions/Ellipse 30 (3).png" size="xs" />Bonnie Green
      <Button>Add</Button>
    </ListgroupItem>
  </Listgroup>
