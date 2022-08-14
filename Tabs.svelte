<script>
import { createEventDispatcher } from "svelte";
const dispatch = createEventDispatcher();
export let items;
export let activeItem;
</script>

<div class="tabs">
<ul>
{#each items as item}
<li on:click={() => dispatch('tabChange', item)}>
<div class:active={item === activeItem} class:hidden={item === "Home"}>{item}</div>
</li>
{/each}
</ul>

</div>

<style>
  ul {
    display: flex;
    float: right;
    justify-content: right;
    list-style-type: none;
    cursor: pointer;
    margin: 0px;
  }

  li {
    margin: 0 16px;
    font-family: roboto condensed;
    font-weight: 200;
    font-size: 17px;
  }
  .active {
    border-bottom: 1px solid;
  }
  .hidden {
    display: none;
  }
</style>