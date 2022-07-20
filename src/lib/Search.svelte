<script>
</script>

<div class="search">
	<input id="search-field" type="text" placeholder="Search" />
	<button class="search-btn">Search</button>
</div>

<style>
	.search {
    width: fit-content;
		margin: 120px auto 0;
    display: flex;
	}
	#search-field {
		background-color: transparent;
		border: 2px solid white;
		border-radius: 24px 0 0 24px;
		border-right: none;
		color: white;
		font-size: 24px;
		line-height: 24px;
		padding: 16px 24px;
		max-width: 800px;
		width: 60vw;
	}
	.search-btn {
		background-color: black;
		text-align: center;
		font-size: 24px;
		border-radius: 0 24px 24px 0;
		width: calc(70vw / 6);
		max-width: 200px;
    color: white;
	}
  .search-btn:hover{
    cursor: pointer;
    background-color: #222;
  }
</style>
