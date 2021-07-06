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
        width: calc(100% / 3);
    }
</style>

<div class="container">
    <div>
        <Card image="https://via.placeholder.com/320x180/" link="https://google.com" linkTitle="Link">
            <h3 slot="title">Title</h3>
            <p slot="description">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Commodi, ratione!</p>
        </Card>
    </div>
</div>