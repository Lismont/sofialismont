<script>
import { fade } from "svelte/transition";
</script>


<div p in:fade="{{duration: 2000 }}" out:fade>Ich habe Erfahrung mit verschiedenen Institutionen, u.A. das Goetheanum, die Gallerie Kubus und eine Synagoge in
	Hegenheim. Ich spreche Deutsch, Französische, Russisch, Estnisch und Spanisch</div>

<style>
  div {
    font-family: "roboto condensed";
    font-weight: 400;
    font-size: 25px;
    color: #1b1b1b;
    text-align: left;
    margin-left: 15%;
    margin-right: 15%;
    margin-top: 100px;
    margin-bottom: 50px;
  }
</style>