<script lang="ts">
    import {Button, Menu, Container, Link, Item, Segment, Header, Table, Table_Body, Table_Col, Table_Row, Icon, Message, Content, Column, Image } from 'svelte-fomantic-ui';

    import roy from "./assets/roy.jpeg"

    let page = "why";
</script>

<main>
    <Segment ui inverted vertical center aligned style="min-height:1000px">
        <Container ui>
            <Menu ui large secondary inverted pointing>
                <Link item active={page==="start"} blue={page==="start"} on:click={()=>page="start"}>Start</Link>
                <Link item active={page==="who"} blue={page==="who"} on:click={()=>page="who"}>About Me</Link>
                <!-- <Link item active={page==="what"} blue={page==="what"} on:click={()=>page="what"}>What</Link> -->
                <Link item active={page==="strong_ideas"} blue={page==="strong_ideas"} on:click={()=>page="strong_ideas"}>Strong Ideas</Link>
                <Link item active={page==="quadruple"} blue={page==="quadruple"} on:click={()=>page="quadruple"}>Quadruple Diamond</Link>
                <Menu right>
                    <Link item active={page==="contact"} green={page==="contact"} on:click={()=>page="contact"}>Contact</Link>
                </Menu>
            </Menu>
        </Container>
        {#if page==="start"}
            <Container ui style="padding-top:50px;min-height:200px;padding-bottom:50px;">
                <Header ui h2 inverted>Welcome to the homepage of 'Dr. Roy' <br><span style="font-size:14px">(he/him)</span></Header>
                <Header ui h3 inverted>Calm Technologist and Mixed Reality Expert.</Header>
                {#if page==="start"}
                    <Message ui icon compact blue>
                        <Icon ui lightbulb/>
                        <Content>
                            <Header ui h4 style="font-style:italic">The greatest achievement of humankind is to be able to think and propogate ideas.</Header>
                            <Header ui h4 style="font-style:italic">&nbsp;</Header>
                            <Header ui h4 style="font-style:italic">All that we leave behind us, are the ideas we helped grow during our lifetimes.</Header>
                            <Header ui h4 style="font-style:italic">&nbsp;</Header>
                            <Header ui h4 style="font-style:italic">For the future of humankind, we must all learn to grow strong ideas.</Header>
                        </Content>
                    </Message>
                {/if}
            </Container>
        {:else if page==="who"}
            <Container ui grid style="padding-top:50px;min-height:200px;padding-bottom:50px;">
                <Column four wide>
                    <Image ui src={roy}/>
                    <span style="font-style:italic">Dr. Roy C. Davies</span>
                </Column>
                <Column twelve wide justified>
                    I've been in and out of the academic world for three and half decades now.  My PhD work was on the Usability of Virtual Reality for brain injury rehabilitation and participatory design.  This was in the early days of VR.
                    Sometimes, students, especially those with English as a second language, call me 'Dr. Roy' rather than 'Dr. Davies'.  I kinda like it, so I don't discourage it - it's both formal and informal at the same time.
                    <br><br>
                    I've built a few companies, and together with my academic experience, I've grown a deep understanding of how to grow strong ideas for both commercial and academic purposes.  This is my key driving force - to help people to learn how to grow strong ideas.  Anybody can do it with a bit of training - something I've learned working for academyEX.
                    <br><br>
                    There are several tasks that keep me occupied.  First and foremost, there is my family, which sits above all else.  My day job is as a Senior Technician at the Smart Digital Lab in the University of Auckland, Department of Civil and Environmental Engineering.
                    I have a few side hustles - consulting tasks that allow me to impart my knowledge and experience to others (and promote the strong ideas methodology), in particular with academyEX where I advise Masters students, and a few startups where I act as a 'Technology Friend' - helping people to understand and work with technical teams.
                    <br><br>
                 </Column>
                <Column sixteen wide justified>
                    <Header ui h4 inverted>Growing strong ideas</Header>
                    What is a strong idea?  We often think of ideas as 'good' or 'bad', evaluating them based on our personal values.  But before that, we need to grow an idea to its full strength, finding all its weaknesses, and casting aside those that are not strong enough.
                    In science, this is called 'conjecture and refutation', and was first formulated by Karl Popper.  A similar technique is used in open-source communities with the pull-request process, and in business with the lean startup methodology.
                    <br><br>
                    Common to these is the need to formulate an idea, then test it to breaking point.  The idea is conjectured, then we work hard to attempt to refute it.  If it continually survives, it is a strong idea.  If it does not, we learn from the experience and try again.
                    <br><br>
                    In refuting ideas, it is critical that a wide range of viewpoints are covered.  Ideally this is done by a diverse group of people with a variety of world views and backgrounds.
                </Column>
                <Column sixteen wide justified>
                    <Header ui h4 inverted>A new technology paradigm - mixing realities</Header>
                    The world is going through a paradigm shift in technology.  We are transitioning from the information age to the intelligence age.  Further, the nature of our interactions with technology is changing.  Now, technology is more able to communicate with us in ways that are natural to human beings.
                    This means that we are finally moving away the desktop metaphor to the objects and actors metaphor.  This is part of spatial computing, meaning that intelligent devices and virtual entities are all around us, working with us in a supportive, augmenting manner.
                    <br><br>
                    At least, that is the dream.  Humans, of course, will find interesting and inventive ways to pervert this ideal, so active work in ethics, privacy and security is necessary.
                </Column>
                <Column sixteen wide justified>
                    <Header ui h4 inverted>Universal design (and calm technology)</Header>
                    A promising area is the use of emerging technologies for assistive devices.  This is a natural fit, as the technology is able to adapt to the user, rather than the user having to adapt to the technology.  All people, regardless of physical and cognitive capability, should be able to take part in society as equals.  Alas, today, that is not so, but adaptive and adaptable calm technologies may be part of the answer.
                    <br><br>
                    Universal design is often touted as a way forward, but in reality, it is impossible to design for all.  However, with care, we can design for the majority, and technology can adapt itself to meet the needs and preferences of the individual.
                </Column>
                <Column sixteen wide justified>
                    So, that's me in a few paragraphs.  The rest of this website has more detail - I hope you find it interesting and inspiring.  In case you are wondering, this site was built using svelte vite, and a library I created called svelte-fomantic-ui.
                </Column>
            </Container>
        {:else if page==="what"}
            <Container ui style="padding-top:50px;min-height:200px;padding-bottom:50px;">
                <Header ui h2 inverted>What</Header>
            </Container>
            <Container ui>

            </Container>
        {:else if page==="strong_ideas"}
            <Container ui grid style="padding-top:50px;min-height:200px;padding-bottom:50px;">
                <Column sixteen wide>
                    <Header ui h3 inverted>Growing Strong Ideas</Header>
                 </Column>
                 <Column sixteen wide>
                    This is a little story I created for students I work with to help them understand better what it means to grow strong ideas.  <Link ui href="https://www.linkedin.com/in/priyan-jayamaha-16655316/">Priyan Jayamaha</Link>, created the fantastic illustrations.
                 </Column>
                <Column sixteen wide left aligned>
                    <div style="position:relative;width:100%;height:0;padding-bottom:calc(56.25% + 40px);"><iframe allowfullscreen style="position:absolute; width: 100%; height: 100%;border: solid 1px #333;" src="https://www.beautiful.ai/embed/-N_0NfqlHyRmYIUWL_-O?utm_source=beautiful_player&utm_medium=embed&utm_campaign=-Mv_W94JHHhsVB3uEVZc"></iframe><a href="https://www.beautiful.ai/embed/-N_0NfqlHyRmYIUWL_-O?utm_source=beautiful_player&utm_medium=embed&utm_campaign=-Mv_W94JHHhsVB3uEVZc">View The story of hine on Beautiful.ai</a></div>
                </Column>
            </Container>
        {:else if page==="contact"}
            <Container ui style="padding-top:50px;min-height:200px;padding-bottom:50px;">
                <Header ui h2 inverted>You can find me in various places</Header>
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
                            <Table_Col right aligned>Academia <Icon ui scroll/></Table_Col>
                            <Table_Col><Link href="https://roydavies12.academia.edu" target="_blank">https://roydavies12.academia.edu</Link></Table_Col>
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
