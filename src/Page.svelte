<script>
	export let user;
</script>

<div class="main">
        <h1>{user.name}</h1>
	    <p>{user.description}</p>
    <div class="socialmedia">
        {#each user.socialmedia as socialmedia}
            <span><a class="{socialmedia.key}" target="_blank" href="{socialmedia.value}">{socialmedia.key}</a></span>
        {/each}
    </div>
</div>

<style>
	.main {
        display: flex !important;
	text-align: center;
	padding-top: 25em;
        flex-direction: column;
        justify-content: center;
        align-items: center;
	}

    a {
        font-size: 20px; 
        list-style: none;
        text-decoration: none;
        cursor: pointer;
        transition: font-size 550ms ease, color 1ms ease;
        background-color: #5865F2;
        color: #fff;
        padding-top: 5px;
        padding-bottom: 5px;
        padding-left: 10px;
        padding-right: 10px;
        border-radius: 50px;
    }

    .socialmedia {
        padding-top: 25px;
    }

    span {
        padding-right: 10px;
    }

    a:hover {
        font-size: 30px;   
        color: #5865F2;
        background-color: #fff;
    }

    @media (max-width: 1000px) {
    .main {
        display: flex !important;
	padding-top: 20em !important;
	}
    }

</style>
