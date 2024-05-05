<script>
    import LogoTextLightWithVersion from "./logo/logo_text_light_with_version.svelte";
    import { _ } from "svelte-i18n";
</script>

<footer
    class="bg-footer-background text-white w-full grid grid-cols-2 md:grid-cols-3 gap-y-8 gap-x-12 p-12 mt-12 rounded-t-3xl"
>
    <div class="col-span-2 md:col-span-1">
        <LogoTextLightWithVersion></LogoTextLightWithVersion>
    </div>
    <div>
        <h5 class="font-semibold"><a href="https://www.pttkstaszow.info/">PTTK Staszów</a></h5>
    </div>
    <div>
        <h5 class="font-semibold">Based on <a href="https://github.com/Flomp/wanderer">wanderer</a></h5>
    </div>
</footer>

<style>
    footer li:not(:last-child) {
        margin-bottom: 4px;
    }
</style>
