<script>
  import { url } from "@sveltech/routify";
</script>

<h3>Forgot Password</h3>
<p>Please provide required information below.</p>
<form action="">
  <div class="form-group">
    <label for="">Email or Mobile number</label>
    <input type="text" class="form-control" />
  </div>
  <div class="pt-2">
    <button class="btn btn-block btn-primary">Submit</button>
  </div>
  <div class="pt-3 d-flex">
    <div class="text-left">
      <a href={$url('/')}>Back to login</a>
    </div>
    <div class="flex-grow-1" />
    <div class="text-right">
      <a href={$url('/register')}>Create an account</a>
    </div>
  </div>
</form>
