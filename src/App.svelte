<script>
  import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
  import { Carousel } from 'flowbite-svelte';
  import suspicaciasLogo from "./assets/suspicacias.ico"
  import { AddressBookOutline } from 'flowbite-svelte-icons';
  import {images} from './images.js'
  
</script>




<main class="">
  <Navbar fluid="true">
    <NavBrand href="/">
      <img src={suspicaciasLogo} class="me-3 h-6 sm:h-9" alt="Flowbite Logo" />
      <span class="self-center whitespace-nowrap text-xl font-semibold text-red-600">Suspicacias</span>
    </NavBrand>
    <NavHamburger menuClass="dark:text-red-600"/>
    <NavUl>
      <NavLi href="/">Inicio</NavLi>
      <NavLi href="/productos">Productos</NavLi>
      <NavLi href="/contacto">Contacto</NavLi>
    </NavUl>
  </Navbar>
  <div class="">
    <Carousel class="sm:h-screen xl:h-18" {images} let:Controls imgClass="h-full w-fit rounded-sm">
      <Controls />
    </Carousel>
  </div>  
  <h1>texto por aca</h1>
</main>


<style>
</style>
