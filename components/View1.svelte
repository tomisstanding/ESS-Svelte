<script>
  let showModal = false;
  function showAnswer() {
    this.nextElementSibling.style.display = 'block';
    (!showModal) ? console.log('asf') : ('asdfsd')
  };
  function closeModal() {
    this.parentNode.style.display = 'none';
  }
</script>

<main>
  <section id="section-1">
    <h1>Knowledge Check</h1>
    <p>Click on each word to review it's definition</p>
   <div class="tile-wrapper">
      <div class="tile" on:click={showAnswer}><span>Consumer</span></div>
      <div class="answer">A person 21 years of age or older who purchases marijuana or marijuana products for personal use by persons 21 years of age or older, but not for resale to others. <button on:click={closeModal}>X</button></div>
      <div class="tile" on:click={showAnswer}>Consumption</div>
      <div class="answer">A person 21 years of age or older who purchases marijuana or marijuana products for personal use by persons 21 years of age or older, but not for resale to others.<button on:click={closeModal}>X</button></div>
      <div class="tile" on:click={showAnswer}>Marijuana</div>
      <div class="answer">The act of ingesting, inhaling, or otherwise introducing marijuana into the human body.<button on:click={closeModal}>X</button></div>
      <div class="tile" on:click={showAnswer}>Marijuana Accessories</div>
      <div class="answer">All parts of the plant of the genus cannabis whether growing or not, the seeds thereof, the resin extracted from any part of the plant, and every compound, manufacture, salt, derivative, mixture, or preparation of the plant, its seeds, or its resin, including marijuana concentrate. Marijuana does not include fiber produced from the stalks, oil, or cake made from the seeds of the plant, sterilized seed of the plant which is incapable of germination, or the weight of any other ingredient combined with marijuana to prepare topical or oral administrations, food, drink, or other products.<button on:click={closeModal}>X</button></div>
      <div class="tile" on:click={showAnswer}>Marijuana Cultivation Facility</div>
      <div class="answer">Any equipment, products, or materials of any kind which are used, intended for use, or designed for use in planting, propagating, cultivating, growing, harvesting, composting, manufacturing, compounding, converting, producing, processing, preparing, testing, analyzing, packaging, repackaging, storing, vaporizing, or containing marijuana, or for ingesting, inhaling, or otherwise introducing marijuana into the human body.<button on:click={closeModal}>X</button></div>
      <div class="tile" on:click={showAnswer}>Marijuana Establishment</div>
      <div class="answer">A marijuana cultivation facility, a marijuana testing facility, a marijuana product manufacturing facility, or a retail marijuana store.<button on:click={closeModal}>X</button></div>
      <div class="tile" on:click={showAnswer}>Marijuana Product Manufactoring Facility</div>
      <div class="answer">An entity registered to purchase marijuana; manufacture, prepare, and package marijuana products; and sell marijuana and marijuana products to other marijuana product manufacturing facilities and to retail marijuana stores, but not to consumers.<button on:click={closeModal}>X</button></div>
      <div class="tile" on:click={showAnswer}>Marijuana Products</div>
      <div class="answer">Concentrated marijuana products and marijuana products that are comprised of marijuana and other ingredients and are intended for use or consumption, such as, but not limited to, edible products, ointments, and tinctures.<button on:click={closeModal}>X</button></div>
      <div class="tile" on:click={showAnswer}>Marijuana Testing Facility</div>
      <div class="answer">An entity registered to analyze and certify the safety and potency of marijuana. <button on:click={closeModal}>X</button></div>
      <div class="tile" on:click={showAnswer}>Retail Marijuana Store</div>
      <div class="answer">An entity registered to purchase marijuana from marijuana cultivation facilities, to purchase marijuana and marijuana products from marijuana product manufacturing facilities, and to sell marijuana and marijuana products to consumers. <button on:click={closeModal}>X</button></div>
    </div>
  </section>
</main>

<style>

</style>
