<script>
    import { logLevels } from "@/utils/CommonHelper";

    let classes = "";
    export { classes as class }; // export reserved keyword
</script>

<div class={classes}>
    默认日志级别:
    <div class="inline-flex flex-gap-5">
        {#each logLevels as options}
            <code class="txt-xs">{options.level}:{options.label}</code>
        {/each}
    </div>
</div>
