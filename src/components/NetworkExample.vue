<template>
  <v-network-graph :nodes="nodes" :edges="edges" />
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {
    const nodes = {
      node1: { name: "Node 1" },
      node2: { name: "Node 2" },
      node3: { name: "Node 3" },
      node4: { name: "Node 4" },
    };
    const edges = {
      edge1: { source: "node1", target: "node2" },
      edge2: { source: "node2", target: "node3" },
      edge3: { source: "node3", target: "node4" },
    };
    return { nodes, edges };
  },
});
</script>
