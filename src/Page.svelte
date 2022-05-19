<script>
	export let user;
</script>

<div class="main">
        <h1>{user.name}</h1>
	    <p>{user.description}</p>
    <div class="socialmedia">
        <span><a class="instagram" target="_blank" href="{user.socialmedia.instagram}">İnstagram</a></span>
        <span><a class="github" target="_blank" href="{user.socialmedia.github}">GitHub</a></span>
        <span><a class="discord" target="_blank" href="{user.socialmedia.discord}">Discord</a></span>
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
        transition: font-size 550ms ease, color 550ms ease;
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

</style>