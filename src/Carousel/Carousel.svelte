<script>
    import {
        Carousel,
        CarouselControl,
        CarouselIndicators,
        CarouselItem,
        CarouselCaption,
    } from "sveltestrap";

    const items = [
        {
            url:
                "https://images.unsplash.com/photo-1494599948593-3dafe8338d71?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80",
            title: "Welcome to learn Programming Languages Here!",
            subTitle:
                "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Rem expedita, neque nihil eius et assumenda! Libero vero magnam cumque voluptatum aut, commodi tenetur maxime incidunt fuga ea asperiores ab autem!",
        },
        {
            url:
                "https://images.unsplash.com/photo-1456244797041-024e2abaf31c?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80",
            title: "Learn Programming Languages From Zero to Hero!",
            subTitle:
                "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Rem expedita, neque nihil eius et assumenda! Libero vero magnam cumque voluptatum aut, commodi tenetur maxime incidunt fuga ea asperiores ab autem!",
        },
        {
            url:
                "https://images.unsplash.com/photo-1567360014060-340d3599a017?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=750&q=80",
            title: "Learn Programming Languages with an Experiential Mentor",
            subTitle:
                "Lorem, ipsum dolor sit amet consectetur adipisicing elit. Rem expedita, neque nihil eius et assumenda! Libero vero magnam cumque voluptatum aut, commodi tenetur maxime incidunt fuga ea asperiores ab autem!",
        },
    ];
    let activeIndex = 0;
</script>

<Carousel {items} bind:activeIndex ride={true} interval={2000}>
    <CarouselIndicators bind:activeIndex {items} />

    <div class="carousel-inner">
        {#each items as item, index}
            <CarouselItem bind:activeIndex itemIndex={index}>
                <img
                    src={item.url}
                    class="d-block w-100"
                    height="600"
                    alt={item.title}
                />
                <CarouselCaption
                    class="text-dark"
                    captionHeader={item.title}
                    captionText={item.subTitle}
                />
            </CarouselItem>
        {/each}
    </div>

    <CarouselControl direction="prev" bind:activeIndex {items} />
    <CarouselControl direction="next" bind:activeIndex {items} />
</Carousel>
