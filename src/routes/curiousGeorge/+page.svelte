  
  <script>
    import { Listgroup, ListgroupItem, Button, Avatar } from 'flowbite-svelte';
    // import { SocialIcons } from 'flowbite';

    const socialLinks = [
    { icon: 'facebook', url: 'https://facebook.com/yourpage' },
    { icon: 'twitter', url: 'https://twitter.com/yourhandle' },
    // Add more social media links as needed
  ];
  </script>
  
  <Listgroup active class="w-48">
    <h3 class="p-1 text-center text-xl font-medium text-gray-900 dark:text-white">Suggestions</h3>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">Based in</h5>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">Skills</h5>
      <p>A 3D model of a yellow banana with textures and a UV Map</p>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">Languages</h5>
      <p>2673901020</p>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2">
      <h5 class="uppercase">socials</h5>
     <!-- <SocialIcons {links={socialLinks}} /> -->
    </ListgroupItem>
  </Listgroup>
