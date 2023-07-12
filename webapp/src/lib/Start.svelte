<script lang="ts">
    import { Container, Header, Icon, Message, Content } from "svelte-fomantic-ui";

    export let page = "start";
</script>

<Container ui style="padding-top:50px;min-height:200px;padding-bottom:50px;">
    <Header ui h2 inverted>Welcome to the professional webpage of 'Dr. Roy' <br><span style="font-size:14px">(he/him)</span></Header>
    <Header ui h3 inverted>Calm Technologist and Mixed Reality Expert</Header>
    {#if page==="start"}
        <Message ui icon compact blue>
            <Icon ui lightbulb/>
            <Content>
                <Header ui h4 style="font-style:italic">The greatest achievement of humankind is to be able to think and propogate ideas.</Header>
                <Header ui h4 style="font-style:italic">&nbsp;</Header>
                <Header ui h4 style="font-style:italic">All that we leave behind us, are the ideas we helped grow during our lifetimes.</Header>
                <Header ui h4 style="font-style:italic">&nbsp;</Header>
                <Header ui h4 style="font-style:italic">For the future of humankind, we must all learn to grow strong ideas that benefit our societies and the planet.</Header>
            </Content>
        </Message>
    {/if}
</Container>
