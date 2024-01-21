  
  <script>
    import { Listgroup, ListgroupItem, Button, Avatar } from 'flowbite-svelte';
    import Us_flag from '$lib/images/Frame 15.png';
    import Twitter from '$lib/images/Vector.png';
    import Instagram from '$lib/images/Vector (1).png';
    import What from '$lib/images/Vector (2).png';
    import Linkedin from '$lib/images/Vector (3).png';
    import Youtube from '$lib/images/Vector (4).png';
    // import { SocialIcons } from 'flowbite';

    const curious = [
      { title: "BASED IN", content: "US Flag" },
      { title: "SKILLS", content: "Abobe Photoshop, After Effects, Blender, Content Creation" },
      { title: "LANGUAGES", content: "English, French" },
      { title: "ACCOUNT CREATED ON", content: "December 12, 2022" },
      { title: "SOCIALS", content: "Icons" },
    ];

  </script>
  
  <Listgroup active class="w-100% border-none" style="background: #282828;">
    <h3 class="p-3 text-xl font-medium text-gray-900 uppercase" style="color: #FF8A00; font-size: 20px;">About Curious George</h3>
    <ListgroupItem class="text-base font-semibold gap-2 border-none hover:bg-primary-1">
      <div>
        <h5 class="uppercase" style="font-size: 17px; color: white">{curious[0].title}</h5>
        <img src={Us_flag} alt="Flag">
      </div>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2 border-none hover:bg-primary-1">
      <div>
        <h5 class="uppercase" style="font-size: 17px; color: white">{curious[1].title}</h5>
        <p style="font-size: 10px; color: white; opacity: 60%;">{curious[1].content}</p>
      </div>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2 border-none hover:bg-primary-1">
      <div>
        <h5 class="uppercase" style="font-size: 17px; color: white">{curious[2].title}</h5>
        <p style="font-size: 10px; color: white; opacity: 60%;">{curious[2].content}</p>
      </div>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2 border-none hover:bg-primary-1">
      <div>
        <h5 class="uppercase" style="font-size: 17px; color: white">{curious[3].title}</h5>
        <p style="font-size: 10px; color: white; opacity: 60%;">{curious[3].content}</p>
      </div>
    </ListgroupItem>
    <ListgroupItem class="text-base font-semibold gap-2 border-none hover:bg-primary-1">
      <div>
        <h5 class="uppercase" style="font-size: 17px; color: white">{curious[4].title}</h5>
        <img src={Youtube} alt="youtube" style="display: inline; padding: 5px; padding-left: 0;"/>
        <img src={What} alt="what" style="display: inline; padding: 5px;"/>
        <img src={Linkedin} alt="linkedin" style="display: inline; padding: 5px;"/>
        <img src={Instagram} alt="instagram" style="display: inline; padding: 5px;"/>
        <img src={Twitter} alt="twitter" style="display: inline; padding: 5px;"/>
      </div>
    </ListgroupItem>
  </Listgroup>
