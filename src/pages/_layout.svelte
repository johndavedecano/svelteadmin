<script>
  import Wrapper from "./../components/Wrapper.svelte";
  import Sidebar from "./../components/Sidebar.svelte";
  import Header from "./../components/Header.svelte";
  import Footer from "./../components/Footer.svelte";
</script>

<style>
  .auth {
    display: flex;
    flex: 1;
    flex-direction: column;
    background: var(--primary); /* fallback for old browsers */
    background: -webkit-linear-gradient(
      to right,
      var(--purple),
      var(--primary)
    ); /* Chrome 10-25, Safari 5.1-6 */
    background: linear-gradient(
      to right,
      var(--purple),
      var(--primary)
    ); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
  }

  .auth__content {
    flex: 1;
    display: flex;
    justify-content: center;
    padding-top: 150px;
  }
</style>

<Wrapper>
  <div class="auth">
    <div class="auth__content">
      <div class="col-md-4">
        <div class="card border-none">
          <div class="card-body">
            <div class="p-4">
              <slot />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</Wrapper>
