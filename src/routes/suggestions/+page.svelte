  
  <script>
    import { Listgroup, ListgroupItem, Avatar, Button } from 'flowbite-svelte';
    import Ellipse1 from "$lib/images/suggestions/Ellipse 30 (1).png";
    import Ellipse2 from "$lib/images/suggestions/Ellipse 30 (2).png";
    import Ellipse3 from "$lib/images/suggestions/Ellipse 30 (3).png";
    import Ellipse4 from "$lib/images/suggestions/Ellipse 30 (4).png";
    import Ellipse5 from "$lib/images/suggestions/Ellipse 30 (5).png";
    import Ellipse6 from "$lib/images/suggestions/Ellipse 30 (6).png";
    import Ellipse7 from "$lib/images/suggestions/Ellipse 30 (7).png";
    import Ellipse8 from "$lib/images/suggestions/Ellipse 30 (8).png";
    import Ellipse9 from "$lib/images/suggestions/Ellipse 30 (9).png";
  </script>
  
  <Listgroup active class="w-48">
    <h3 class="p-1 text-center text-xl font-medium text-gray-900 dark:text-white">Suggestions</h3>
    <ListgroupItem class="text-base font-semibold gap-2">
      <Avatar src={Ellipse1} size="xs" />Jese Leos
      <Button>Add</Button>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <Avatar src={Ellipse2} size="xs" />Robert Gouth
      <Button>Add</Button>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <Avatar src={Ellipse3} size="xs" />Bonnie Green
      <Button>Add</Button>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
        <Avatar src={Ellipse4} size="xs" />Bonnie Green
        <Button>Add</Button>
      </ListgroupItem>
      <ListgroupItem class="text-base font-semibold gap-2">
        <Avatar src={Ellipse5} size="xs" />Bonnie Green
        <Button>Add</Button>
      </ListgroupItem>
      <ListgroupItem class="text-base font-semibold gap-2">
        <Avatar src={Ellipse6} size="xs" />Bonnie Green
        <Button>Add</Button>
      </ListgroupItem>
      <ListgroupItem class="text-base font-semibold gap-2">
        <Avatar src={Ellipse7} size="xs" />Bonnie Green
        <Button>Add</Button>
      </ListgroupItem>
      <ListgroupItem class="text-base font-semibold gap-2">
        <Avatar src={Ellipse8} size="xs" />Bonnie Green
        <Button>Add</Button>
      </ListgroupItem>
      <ListgroupItem class="text-base font-semibold gap-2">
        <Avatar src={Ellipse9} size="xs" />Bonnie Green
        <Button>Add</Button>
      </ListgroupItem>
  </Listgroup>
