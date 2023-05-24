<script lang="ts">
    export let emoji: string;
    export let type: "svg" | "png" = "svg";
    export let exClass: string = "";
    export let exStyle: string = "width: 32px; height: 32px;";
    export let baseURL = "https://twemoji.naecqde.workers.dev/twemoji/";

    const url = `${baseURL}${emoji}.${type}`;
</script>

<img class={exClass} src={url} alt={emoji} style={exStyle} />
