<script>
    import Card from './Card.svelte'
</script>

<style>
    .container {
        width: 100%;
        display: flex;
        justify-content: center;
    }
    .container > div {
        width: calc(97% / 3);
        margin: 0 1%;
    }
    a {
        padding: 7px 20px;
        text-decoration: none;
        border: 1px solid silver;
        border-radius: 10px;
        color: white;
        background-color: darkcyan;
        transition: .3s;
    }

    a:hover {
        filter: brightness(110%);
        transform: scale(1.1);
    }
</style>

<div class="container">
    <div>
        <Card image="https://via.placeholder.com/320x180/" link="https://google.com" linkTitle="Link">
            <h3 slot="title">Title</h3>
            <p slot="description">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Commodi, ratione!</p>
        </Card>
    </div>
    <div>
        <Card image="https://via.placeholder.com/320x180/">
            <h3 slot="title">Title 2</h3>
            <p slot="description">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Commodi, ratione!</p>
            <a slot="link" href="https://google.com">Link</a>
        </Card>
    </div>
</div>