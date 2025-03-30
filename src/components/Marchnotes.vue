<script>
export default {
    name: "Marchnotes",
    data() {
        return {
            articles: [
                {
                    title: "IntersectionObserver",
                    link: "https://www.debugbear.com/blog/lazy-load-background-images-intersection-observer",
                    description: "Met de IntersectionObserver API achtergrondafbeeldingen kunt lazy loaden. Deze API detecteert wanneer elementen in beeld komen, waardoor je afbeeldingen pas laadt zodra ze nodig zijn, wat de prestaties verbetert.",
                    image: ""
                },
                {
                    title: "Een smooth border-radius animation met view-transitions",
                    link: "https://www.bram.us/2025/03/11/view-transitions-border-radius",
                    description: "Ipv het vervagen van snapshots wordt ::view-transition-group toegevoegd voor een smooth transition. Wel overflow: clip gebruiken om te voorkomen dat snapshots bleed out.",
                    image: "/src/assets/smooth-border-radius.png"
                }
            ],
            cacheInfo: null
        };
    },
    created() {
        this.loadCacheInfo();
    },
    methods: {
        loadCacheInfo() {
            this.cacheInfo = {
                title: "Wat is cache?",
                description: "Wanneer een website wordt geopend, slaat de browser een kopie van bepaalde onderdelen van de site op...",
                types: [
                    {
                        name: "Browser-cache",
                        info: "Bij elk bezoek slaat je browser elementen van de website op in de cache. Dit zorgt ervoor dat de website sneller laadt bij een volgend bezoek."
                    },
                    {
                        name: "Server-cache",
                        info: "Een server-cache slaat tijdelijk kopieën van webpagina’s of gegevens op de server op, zodat deze sneller kunnen worden geladen."
                    }
                ],
                article: `
                    <article>
                        <h2>Cache</h2>
                        <p>Wanneer een website wordt geopend, slaat de browser een kopie van bepaalde onderdelen van de site op in de cache. Dit wordt gedaan om de laadtijd te verkorten en de gebruikerservaring te verbeteren. Als je dezelfde website later opnieuw bezoekt, kan de browser deze opgeslagen kopie (cache) gebruiken in plaats van alles opnieuw te downloaden. Hierdoor zijn recente wijzigingen op een website soms niet direct zichtbaar. Cache is een tijdelijk opgeslagen kopie.</p>
                        
                        <h3>Soorten cache:</h3>
                        <ul>
                            <li><strong>Browser-cache</strong>: Bij elk bezoek slaat je browser elementen van de website op in de cache. Dit zorgt ervoor dat de website sneller laadt bij een volgend bezoek. Soms is het nodig om de browser-cache te legen om recente wijzigingen op een website te zien.</li>
                            <li><strong>Server-cache</strong>: Een server-cache slaat tijdelijk kopieën van webpagina’s of gegevens op de server op. Dit zorgt ervoor dat de server sneller kan reageren op verzoeken, omdat deze niet steeds dezelfde gegevens opnieuw hoeft te genereren. Deze cache wordt lokaal op de server opgeslagen of verspreid over meerdere servers.</li>
                        </ul>
                        <p>Cache is cruciaal omdat het de laadtijd van websites verkort, het dataverbruik vermindert en de belasting van de server verlaagt. Doordat gegevens lokaal zijn opgeslagen, hoeft de server minder vaak dezelfde informatie op te halen.</p>
                        
                        <h3>Hoe verwijder je cache?</h3>
                        
                        <h4>Incognitomodus</h4>
                        <p>De incognitomodus is een browserfunctie waarmee je privé op het internet kunt surfen. In deze modus worden geen eerder opgeslagen gegevens zoals cookies, cache of browsergeschiedenis gebruikt. Dit betekent dat je altijd de meest recente versie van een website ziet, zonder invloed van oude gegevens. Nadat je de modus hebt gebruikt, worden je lokale browsegegevens automatisch gewist.</p>
                        
                        <h4>Browsercache</h4>
                        <p>Je kunt de cache eenvoudig zelf wissen. Klik met de rechtermuisknop terwijl de gewenste site openstaat en selecteer 'Inspect' in het contextmenu. Houd vervolgens de <strong>Ctrl-toets</strong> ingedrukt en klik tegelijkertijd op de <strong>refresh button</strong>. Er verschijnt een menu waarin je de optie <strong>'Empty cache and hard reload'</strong> selecteert. Hiermee wordt je cache gewist.</p>
                        
                        <h5>Chrome</h5>
                        <p>Open eerst Google Chrome en klik op het drie-puntjes-menu <strong>⋮</strong> in de rechterbovenhoek van de browser. Ga naar <strong>Delete Browsing Data</strong>. Vink vervolgens alleen <strong>Cached images and files</strong> aan. Dit bevestig je door op <strong>Delete data</strong> te klikken.</p>
                        
                        <h5>Safari</h5>
                        <p>Open de Safari-instellingen, klik op <strong>Advanced</strong>, en vink onderaan de pagina <strong>Show Develop menu in menu bar</strong> aan. Bovenin verschijnt dan het tabblad <strong>Develop</strong>; klik daarop. Onderin het menu vind je <strong>Empty Caches</strong>, waar je op kunt klikken.</p>
                        
                        <h5>Firefox</h5>
                        <p>Klik op de drie balkjes rechtsboven en kies <strong>History</strong>. Selecteer <strong>Clear recent history</strong> en stel de tijdsperiode in. Vink de optie Cache aan. Klik op <strong>Clear now</strong>. Sluit en heropen Firefox om de wijzigingen toe te passen.</p>
                        
                        <h5>Edge</h5>
                        <p>Klik rechtsboven op het drie-puntjes-menu <strong>⋮</strong> en open <strong>Settings</strong>. Klik dan op <strong>Privacy, Search, and Services</strong>. Onder het kopje <strong>Clear browsing data</strong> vind je <strong>Choose What to Clear</strong>. Als je daarop klikt, kun je <strong>Cached images and files</strong> aanvinken. Klik tot slot op <strong>Clear now</strong> om je cache te wissen.</p>
                        
                        <h4>Server-cache</h4>
                        <p>Een cache-server slaat internetinhoud lokaal op om verzoeken sneller te verwerken. Voor WordPress-sites wordt vaak gebruik gemaakt van een cache-plugin, die het cachen van content beheert. Een plug-in is een tool die je toevoegt aan een programma, zoals WordPress, om nieuwe functies toe te voegen.</p>
                        
                        <h5>Speed Optimizer</h5>
                        <ul>
                            <li>Op SiteGround klik je op Site Tools.</li>
                            <li>Klik vervolgens in de sidebar op <strong>Speed</strong> en daarna op <strong>Caching</strong>.</li>
                            <li>Ga naar <strong>Dynamic Cache</strong> en klik op het <strong>Flush Cache</strong> icoontje onder <strong>Actions</strong> om de cache te verwijderen.</li>
                        </ul>
                        
                        <h5>Cloudflare</h5>
                        <ul>
                            <li>Log in op je Cloudflare-account.</li>
                            <li>Open het dashboard van je website.</li>
                            <li>Ga naar het tabblad "Caching".</li>
                            <li>Klik op "Purge Cache" en kies of je alles of alleen specifieke bestanden wilt wissen.</li>
                        </ul>
                        
                        <h5>WP Super Cache</h5>
                        <ul>
                            <li>Ga in je WordPress-dashboard naar Instellingen &gt; WP Super Cache.</li>
                            <li>Klik op de knop <strong>Cache legen</strong>.</li>
                        </ul>
                        
                        <h5>WP Rocket</h5>
                        <ul>
                            <li>Ga naar Instellingen &gt; WP Rocket.</li>
                            <li>Klik op <strong>Cache opschonen</strong>.</li>
                        </ul>
                        
                        <h4>Bronnen</h4>
                        <ul>
                            <li><a href="https://www.one.com/nl/webhosting/wat-is-een-cache">One.com</a></li>
                            <li><a href="https://www.tundra.nl/vaktaal/cache/">Tundra.nl</a></li>
                            <li><a href="https://www.thisisfever.co.uk/knowledge-hub/what-is-a-browser-cache-and-why-do-i-need-to-clear-it/">This is Fever</a></li>
                            <li><a href="https://its.uiowa.edu/services/how-clear-cache-and-cookies-your-web-browser">University of Iowa</a></li>
                            <li><a href="https://kinsta.com/blog/wordpress-clear-cache/#what-is-caching">Kinsta</a></li>
                        </ul>
                    </article>
                `
            };
        }
    }
};
</script>

<template>
    <div>
        <h1>Notes</h1>
        <p>March 2025</p>

        <section>
            <article v-for="article in articles" :key="article.title">
                <a :href="article.link" target="_blank">
                    <h3>{{ article.title }}</h3>
                </a>
                <p>{{ article.description }}</p>
                <img v-if="article.image" :src="article.image" :alt="article.title" />
            </article>
        </section>

        <section v-if="cacheInfo">
            <h2>{{ cacheInfo.title }}</h2>
            <p>{{ cacheInfo.description }}</p>
            <h3>Soorten cache:</h3>
            <ul>
                <li v-for="type in cacheInfo.types" :key="type.name">
                    <strong>{{ type.name }}:</strong> {{ type.info }}
                </li>
            </ul>
            <div v-html="cacheInfo.article"></div>
        </section>
    </div>
</template>

<style scoped>
    img {
        width: 300px;
    }

</style>
