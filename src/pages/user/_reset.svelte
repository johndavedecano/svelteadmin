<script>
  import Wrapper from "./../../components/Wrapper.svelte";
  import Sidebar from "./../../components/Sidebar.svelte";
  import Header from "./../../components/Header.svelte";
  import Footer from "./../../components/Footer.svelte";
</script>

<style>
  .main {
    display: flex;
    flex: 1;
    flex-direction: column;
  }

  .main__content {
    flex: 1;
  }
</style>

<Wrapper>
  <Sidebar />
  <div class="main">
    <Header />
    <div class="main__content">
      <slot />
    </div>
    <Footer />
  </div>
</Wrapper>
