<script>
    import "../app.pcss";
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger, ImagePlaceholder, Skeleton, TextPlaceholder } from 'flowbite-svelte';
</script>
  
  <div class="relative px-8">
    <Navbar class="px-2 sm:px-4 py-2.5 fixed w-full z-20 top-0 start-0 border-b">
      <NavBrand href="/">
        <img src="/assets/branding/main-logo.png" class="me-3 h-10 sm:h-9" alt="PakBeam Logo" />
      </NavBrand>
      <NavHamburger />
      <NavUl>
        <NavLi href="/experiences" active={true}>Experiences</NavLi>
        <NavLi href="/pak-manager">Pak Manager</NavLi>
        <NavLi href="https://github.com/Unreal-Kingdoms/Pak-Beam/wiki">Docs</NavLi>
        <NavLi href="https://github.com/Unreal-Kingdoms/Pak-Beam">GitHub</NavLi>
      </NavUl>
    </Navbar>
    <div class="content">
        <slot></slot>
    </div>
  </div>