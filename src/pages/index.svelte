<script>
  import { url, goto } from "@sveltech/routify";
</script>

<h3>Welcome Back</h3>
<p>Please provide required information below.</p>

<div class="form-group">
  <label for="">Email or Mobile number</label>
  <input type="text" class="form-control" />
</div>
<div class="form-group">
  <label for="">Password</label>
  <input type="password" class="form-control" />
</div>
<div class="pt-2">
  <button class="btn btn-block btn-primary" on:click={() => $goto('/user')}>
    Submit
  </button>
</div>
<div class="pt-3 d-flex">
  <div class="text-left">
    <a href={$url('/forgot')}>Forgot Password</a>
  </div>
  <div class="flex-grow-1" />
  <div class="text-right">
    <a href={$url('/register')}>Create an account</a>
  </div>
</div>
