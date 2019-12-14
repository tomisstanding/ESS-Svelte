<script>

	let answer = "";

	const showAnswers = () => {
		let answer = document.getElementsByClassName("question");
		let answers = document.getElementsByClassName('answer-container')[0];
		for(let i of answer) {
			i.addEventListener('click', function() {
				answers.style.display = 'block';
			});
		}
	}

	function closeAnswer() {
		let answers = document.getElementsByClassName('answer-container')[0];
		answers.style.display = 'none';
	};

</script>

<section id="section-2">

  <div>
    <h3>Checking IDs Exercise</h3>
    <p>Examine ID to determine whether or not you would sell to the customer. </p>
    <div>
      <img src="https://i.imgur.com/zE5tOlu.jpg" width="400" height="250" alt="">
   	<div class="question">
		<ul>
			<li class="question" on:click={showAnswers} on:click={()=> answer = "INCORRECT"}>SELL</li>
			<li class="question" on:click={()=> answer = "CONGRATS!"}>DON'T SELL</li>
		</ul>
	</div>

	<div class="answer-container">
		<strong>{answer}</strong>
		<p>The correct answer is:</p>
		<strong>DON'T SELL</strong>
		<p>This license has some bumps and scratches indicating that it may have been tampered with. It's expired.</p>
		<button on:click={closeAnswer}>X</button>
	</div>

</section>

<style>
/* OR YOU CAN BLOCK SCOPE CAUSE WHY NOT RIGHT? */
.answer-container {
	display: none;
}
.question {
	cursor: pointer;
	text-decoration: underline;
	color: green;
}
#section-2 {
	background-color: #B2D8B2;
	padding: 20px;
}
.answer-container p {
  margin: 5px auto;
  line-height: 150%;
  font-size: 12px;
}
</style>
