<script>
  import "../../css/app.css";
  import Navbar from '../../components/auth/Navbar.svelte'
  import FooterAuth from '../../components/auth/FooterAuth.svelte'

  const registerBg2 = '../../assets/img/register_bg_2.png';
</script>



<div>
  <Navbar />
  <main>
    <section class="relative w-full h-full py-40 min-h-screen">
      <div
        class="absolute top-0 w-full h-full bg-blueGray-800 bg-no-repeat bg-full"
        style="background-image: url({registerBg2});"
      ></div>
      <slot></slot>
      <FooterAuth absolute="true" />
    </section>
  </main>
</div>
