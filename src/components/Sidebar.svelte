<script>

</script>

<style>
  .sidebar {
    display: flex;
    width: 240px;
    background: var(--gray-dark);
    flex-direction: column;
  }

  .sidebar__top {
    background-color: white;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .sidebar__top .brand {
    font-size: 24px;
    color: var(--purple);
    font-weight: 700;
  }

  .sidebar__top span {
    color: var(--gray);
    font-weight: 700;
  }

  .sidebar__mid {
    flex: 1;
  }

  .sidebar__bottom {
    border-top: solid 1px rgba(109, 118, 126, 0.1);
    height: 60px;
  }

  .navigation {
    display: flex;
    flex-direction: column;
    list-style: none;
    margin: 0;
    padding: 0;
  }

  .navigation li {
    height: 50px;
    display: flex;
    align-items: center;
    border-bottom: solid 1px rgba(109, 118, 126, 0.1);
    padding-left: 15px;
    padding-right: 15px;
    transition: background 1s ease;
  }

  .navigation li a {
    color: var(--gray);
    cursor: pointer;
  }

  .navigation li a:hover,
  .navigation li a:visited {
    text-decoration: none;
  }

  .navigation li:hover {
    background-color: var(--gray);
    color: white;
  }

  .navigation li:hover a {
    color: white;
  }
</style>

<div class="sidebar">
  <div class="sidebar__top">
    <a href="/" class="brand">
      <span>Svelte</span>
      Rocks
    </a>
  </div>
  <div class="sidebar__mid">
    <ul class="navigation">
      <li>
        <a href="/">Dashboard</a>
      </li>
      <li>
        <a href="/">Classes</a>
      </li>
      <li>
        <a href="/">Certificates</a>
      </li>
      <li>
        <a href="/">Exams</a>
      </li>
      <li>
        <a href="/">Transactions</a>
      </li>
      <li>
        <a href="/">Support</a>
      </li>
      <li>
        <a href="/">Account Settings</a>
      </li>
    </ul>
  </div>
  <div class="sidebar__bottom" />
</div>
