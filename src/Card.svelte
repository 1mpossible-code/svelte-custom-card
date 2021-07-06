<div class="container">
    <div class="image">
        <img src={image} alt="320x180">
    </div>
    <div class="under-image">
        <div class="title">
            <slot name="title">
                <h3>Lorem ipsum dolor sit amet.</h3>
            </slot>
        </div>
        <div class="description">
            <slot name="description">
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab aperiam aspernatur culpa dicta dolores
                    et
                    explicabo itaque iure, nisi non numquam omnis, perferendis recusandae sapiente tempore ut
                    voluptatibus!
                    Obcaecati, tempore.</p>
            </slot>
        </div>
        <div class="link">
            {#if link}
                <a href={link}>{linkTitle}</a>
            {:else}
                <slot name="link"/>
            {/if}
        </div>
    </div>
</div>

<style>
    .container {
        border: 1px solid silver;
        width: 100%;
        border-radius: 25px;
        overflow: hidden;
    }

    img {
        width: 100%;
        border-bottom: 1px solid silver;
    }

    .under-image {
        padding: 1rem;
    }

    .title {
        text-align: center;
    }

    .description {
        text-align: justify;
    }

    .link {
        display: flex;
        justify-content: center;
    }

    .link > a {
        padding: 7px 20px;
        text-decoration: none;
        border: 1px solid silver;
        border-radius: 10px;
        color: white;
        background-color: darkcyan;
        transition: .3s;
    }

    .link > a:hover {
        filter: brightness(110%);
        transform: scale(1.1);
    }
</style>

<script>
    export let link;
    export let linkTitle = "Link";
    export let image;
</script>