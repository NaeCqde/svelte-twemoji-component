<script lang="ts">
    export let emoji: string;

    export let type: "svg" | "png" = "svg";
    export let baseURL = "https://twemoji.naecqde.workers.dev/twemoji/";

    let exClass: string = "twemoji";
    let exStyle: string = "";

    export { exClass as class, exStyle as style };

    const url = `${baseURL}${emoji}.${type}`;
</script>

<img class={exClass} src={url} alt={emoji} style={exStyle} />
