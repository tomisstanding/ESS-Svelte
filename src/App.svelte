<script>
	// ~~~~~~~~ IMPORTS ~~~~ //
	import View2 from '../components/View2.svelte'
	import View1 from '../components/View1.svelte'

	let showView2 = false;
	let showView1 = true;

	function toggleView() {
		(showView1)
		? (showView1 = false, showView2 = true)
		: (showView1 = true, showView2 = false)
	}

</script>

<main>

	<h1 id="title"><strong>Page</strong> <small>Knowledge Check: Exercise</small>
    <hr>
  </h1>

 <div class="nav-bar">
    <span>{showView1 ? 'Knowledge Check:' : 'AS 17.37 Medical Uses of Marijuana'} Exercise</span>
    <div>
      <button>Resources</button>
      <div class="resources">
        <a href="#" target="_blank">Alaska Statute 17.37 Medical Uses of Marijuana</a>
        <a href="#" target="_blank">Alaska Statute 17.38 The Regulation of Marijuana</a>
        <a href="#" target="_blank">3 AAC 306 Regulations for the Marijuana Control Board</a>
        <a href="#" target="_blank">Marijuana Handler Permit Application Instructions</a>
      </div>
    </div>
  </div>

	{#if showView2}
		<View2 />
	{:else if !showView2}
		<View1 />
	{/if}

	<button id="navBtn" on:click={toggleView} >
		{showView1 === true ? 'NEXT' : 'BACK'}
	</button>

	<hr>
  <section>
    <h2>Instructions</h2>
    <ul>
      <li> The main document and iframe content each have their own css styles respectively.</li>
      <li> The challenge is to have the same functionality and styling without using an iframe.</li>
      <li>** Make sure your solutions is supported throughout different browsers. **</li>
    </ul>
  </section>

</main>


<style>

</style>

