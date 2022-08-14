<div class="image-grid">
	<img src="./img/eggs.jpg" alt="Eier">
	<img src="./img/forms1.jpg" alt="Formen">
	<img src="./img/taches.jpg" alt="Formen">
	<img src="./img/forms2.jpg" alt="Formen">
	<img src="./img/gitter.jpg" alt="Gitter">
	<img src="./img/portraits.jpg" alt="Portraits">
</div>

<style>
  .image-grid {
    --gap: 10px;
    --num-cols: 3;
    --row-height: auto;
    box-sizing: border-box;
    padding: var(--gap);

    display: grid;
    grid-template-columns: repeat(var(--num-cols), 1fr);
    grid-auto-rows: var(--row-height);
    gap: var(--gap);
    margin-left: 15%;
    margin-right: 15%;
  }

  .image-grid > img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  @media screen and (max-width: 1024px) {
    .image-grid {
      --num-cols: 2;
    }
  }
</style>