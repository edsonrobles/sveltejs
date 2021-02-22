<script>
    import Home from '../layout/Home.svelte';

    const seo = {
        pageName   : '',
        url        : '',
        seo        : '',
        seoImg     : '',
        category   : '',
        keywords   : '',
        description: '',

        facebook     : '',
        twitter      : '',
        FBDescription: '',
        TWDescription: '',

        image: '',
    };
</script>

<svelte:head>
    <title>Svelte JS</title>

    <!-- seo -->
    <!-- generico -->
    <meta name="author" content={seo.pageName} />
    <meta name="keywords" content={seo.keywords} />
    <meta name="description" content={seo.description} />
    <meta name="robots" content="index, follow" />
    <meta http-equiv="cache-control" content="no-cache" />
    <!-- fancy -->
    <meta property="fancy:name" content={seo.pageName} />
    <meta property="fancy:image" content={seo.seo} />
    <meta property="fancy:description" content={seo.description} />
    <meta property="fancy:category" content={seo.category} />
    <!-- global canonical -->
    <link rel="canonical" href={seo.url} />
    <meta property="og:url" content={seo.url} />
    <!-- facebook -->
    <meta name="facebook:site" content={seo.facebook} />
    <meta name="facebook:creator" content={seo.facebook} />
    <meta property="og:type" content="website" />
    <meta property="og:description" content={seo.FBDescription} />
    <meta property="og:image" content={seo.seoImg} />
    <meta property="og:locale" content="es_ES" />
    <!-- twitter -->
    <meta name="twitter:card" content="summary_large_image" />
    <meta name="twitter:site" content={seo.twitter} />
    <meta name="twitter:creator" content={seo.twitter} />
    <meta name="twitter:title" content={seo.pageName} />
    <meta name="twitter:description" content={seo.TWDescription} />
    <meta name="twitter:image" content={seo.seoImg} />
    <!-- datos de open graph -->
    <meta property="og:title" content={seo.pageName} />
    <meta property="og:type" content="article" />
    <meta property="og:url" content={seo.url} />
    <meta property="og:image" content={seo.seoImg} />
    <meta property="og:description" content={seo.description} />
    <meta property="og:site_name" content={seo.pageName} />
    <meta property="og:price:amount" content="" />
    <meta property="og:price:currency" content="C$ Cordoba, U$ Dolar" />
</svelte:head>

<Home />

<style lang="scss">
    @import '../sass/config';
</style>
