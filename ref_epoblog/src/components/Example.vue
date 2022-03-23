<template>
  <div>
    <Markdown :source="source" :plugins="plugins" />
  </div>
</template>

<script>
import markdownItMermaid from 'markdown-it-mermaid'
import Markdown from 'vue3-markdown-it'
import MarkdownText from './example'

export default {
  components: {
    Markdown
  },
  data() {
    return {
      source: MarkdownText,
      plugins: [
        {
          plugin: markdownItMermaid
        }
      ]
    }
  }
}
</script>
