<script lang="ts">
    import {Button, Menu, Container, Link, Item, Segment, Header, Table, Table_Body, Table_Col, Table_Row, Icon, Message, Content, Embed } from 'svelte-fomantic-ui';

    let page = "why";
</script>

<main>
    <Segment ui inverted vertical center aligned style="min-height:1000px">
        <Container ui>
            <Menu ui large secondary inverted pointing>
                <Link item active={page==="why"} blue={page==="why"} on:click={()=>page="why"}>Why</Link>
                <!-- <Link item active={page==="what"} blue={page==="what"} on:click={()=>page="what"}>What</Link> -->
                <Link item active={page==="how"} blue={page==="how"} on:click={()=>page="how"}>How</Link>
                <Menu right>
                    <Link item active={page==="contact"} green={page==="contact"} on:click={()=>page="contact"}>Contact</Link>
                </Menu>
            </Menu>
        </Container>
        {#if page==="why"}
            <Container ui style="padding-top:50px;min-height:200px;padding-bottom:50px;">
                <Header ui h2 inverted>Welcome to the homepage of 'Dr Roy' <span style="font-size:14px">(he/him)</span></Header>
                <Header ui h3 inverted>Calm Technologist and Mixed Reality Expert.</Header>
                {#if page==="why"}
                    <Message ui icon compact blue>
                        <Icon ui lightbulb/>
                        <Content>
                            <Header ui h4 style="font-style:italic">The greatest achievement of mankind is to be able to think and propogate ideas.</Header>
                            <Header ui h4 style="font-style:italic">All that we leave behind are the ideas we helped grow during our lifetimes.</Header>
                            <Header ui h4 style="font-style:italic">For the future of humankind, we must all learn to grow strong ideas.</Header>
                        </Content>
                    </Message>
                {/if}
            </Container>
        <!-- {:else if page==="what"}
            <Container ui style="padding-top:50px;height:200px;">
                <Header ui h2 inverted>What</Header>
            </Container>
            <Container ui>

            </Container> -->


        {:else if page==="how"}
            <Container ui style="padding-top:50px;height:200px;" left aligned>
                <div style="position:relative;width:100%;height:0;padding-bottom:calc(56.25% + 40px);"><iframe allowfullscreen style="position:absolute; width: 100%; height: 100%;border: solid 1px #333;" src="https://www.beautiful.ai/embed/-N_0NfqlHyRmYIUWL_-O?utm_source=beautiful_player&utm_medium=embed&utm_campaign=-Mv_W94JHHhsVB3uEVZc"></iframe><a href="https://www.beautiful.ai/embed/-N_0NfqlHyRmYIUWL_-O?utm_source=beautiful_player&utm_medium=embed&utm_campaign=-Mv_W94JHHhsVB3uEVZc">View The story of hine on Beautiful.ai</a></div>
            </Container>
        {:else if page==="contact"}
            <Container ui style="padding-top:50px;min-height:200px;padding-bottom:50px;">
                <Header ui h2 inverted>You will find me in various places</Header>
                <Table ui inverted centered>
                    <Table_Body>
                        <Table_Row>
                            <Table_Col right aligned>LinkedIn <Icon ui linkedin/></Table_Col>
                            <Table_Col><Link href="https://www.linkedin.com/in/roycdavies/" target="_blank">https://www.linkedin.com/in/roycdavies</Link></Table_Col>
                        </Table_Row>
                        <Table_Row>
                            <Table_Col right aligned>Orcid <Icon ui orcid/></Table_Col>
                            <Table_Col><Link href="https://orcid.org/0000-0001-6302-1931" target="_blank">https://orcid.org/0000-0001-6302-1931</Link></Table_Col>
                        </Table_Row>
                        <Table_Row>
                            <Table_Col right aligned>Research Gate <Icon ui researchgate/></Table_Col>
                            <Table_Col><Link href="https://www.researchgate.net/profile/Roy-Davies-2" target="_blank">https://www.researchgate.net/profile/Roy-Davies-2</Link></Table_Col>
                        </Table_Row>
                        <Table_Row>
                            <Table_Col right aligned>Waipapa Taumata Rau / University of Auckland <Icon ui university/></Table_Col>
                            <Table_Col><Link href="https://profiles.auckland.ac.nz/roy-davies" target="_blank">https://profiles.auckland.ac.nz/roy-davies</Link></Table_Col>
                        </Table_Row>
                        <Table_Row>
                            <Table_Col right aligned>academyEX <Icon ui university/></Table_Col>
                            <Table_Col><Link href="https://academyex.com/people/roy-davies" target="_blank">https://academyex.com/people/roy-davies</Link></Table_Col>
                        </Table_Row>
                        <Table_Row>
                            <Table_Col right aligned>Lunds Universitet / The university of Lund <Icon ui university/></Table_Col>
                            <Table_Col><Link href="https://lup.lub.lu.se/search/person/amt-rda" target="_blank">https://lup.lub.lu.se/search/person/amt-rda</Link> | <Link href="https://www.lu.se/search/roy%20davies" target="_blank">https://www.lu.se/search/roy%20davies</Link></Table_Col>
                        </Table_Row>
                        <Table_Row>
                            <Table_Col right aligned>Imersia <Icon ui tablet alternate/></Table_Col>
                            <Table_Col><Link href="https://www.imersia.com" target="_blank">https://www.imersia.com</Link></Table_Col>
                        </Table_Row>
                        <Table_Row>
                            <Table_Col right aligned>Bitbucket (Imersia) <Icon ui bitbucket/></Table_Col>
                            <Table_Col><Link href="https://bitbucket.org/imersiageneral/cloud-mixed-reality-server-erlang-rel/wiki/Home" target="_blank">https://bitbucket.org/imersiageneral/cloud-mixed-reality-server-erlang-rel/wiki/Home</Link></Table_Col>
                        </Table_Row>
                        <Table_Row>
                            <Table_Col right aligned>Github <Icon ui github/></Table_Col>
                            <Table_Col><Link href="https://github.com/roycdavies" target="_blank">https://github.com/roycdavies</Link> | <Link href="https://github.com/roycdaviesuoa" target="_blank">https://github.com/roycdaviesuoa</Link> | <Link href="https://github.com/uoa-smart-digital-lab" target="_blank">https://github.com/uoa-smart-digital-lab</Link></Table_Col>
                        </Table_Row>
                        <Table_Row>
                            <Table_Col right aligned>Gitlab <Icon ui gitlab/></Table_Col>
                            <Table_Col><Link href="https://gitlab.com/drroycdavies" target="_blank">https://gitlab.com/drroycdavies</Link></Table_Col>
                        </Table_Row>
                        <Table_Row>
                            <Table_Col right aligned>Reality 2.0 <Icon ui globe/></Table_Col>
                            <Table_Col><Link href="https://reality2.ai" target="_blank">https://reality2.ai</Link></Table_Col>
                        </Table_Row>
                        <Table_Row>
                            <Table_Col right aligned>DuckDuckGo Search <Icon ui search/></Table_Col>
                            <Table_Col><Link href="https://duckduckgo.com/?q=roy+davies+virtual+reality+mixed+reality" target="_blank">https://duckduckgo.com/?q=roy+davies+virtual+reality+mixed+reality</Link></Table_Col>
                        </Table_Row>
                    </Table_Body>
                </Table>
            </Container>
        {/if}


    </Segment>

</main>

<style>

</style>
