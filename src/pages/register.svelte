<script>
  import { url, goto } from "@sveltech/routify";
</script>

<h3>Create Account</h3>
<p>Please provide required information below.</p>

<div class="form-group">
  <label for="">Name</label>
  <input type="text" class="form-control" />
</div>

<div class="form-group">
  <label for="">Mobile Number</label>
  <div class="input-group">
    <div class="input-group-prepend">
      <span class="input-group-text">+63</span>
    </div>
    <input type="text" class="form-control" />
  </div>
</div>

<div class="form-group">
  <label for="">Email Address</label>
  <input type="text" class="form-control" />
</div>

<div class="form-group">
  <label for="">Password</label>
  <input type="password" class="form-control" />
</div>

<div class="form-group">
  <label for="">Password Confirmation</label>
  <input type="password" class="form-control" />
</div>
<div class="pt-2">
  <button
    class="btn btn-block btn-primary"
    on:click={evt => {
      evt.preventDefault();
      $goto('/verify');
    }}>
    Submit
  </button>
</div>
<div class="pt-3 d-flex">
  <div class="text-left">
    <a href={$url('/')}>Back to login</a>
  </div>
  <div class="flex-grow-1" />
</div>
