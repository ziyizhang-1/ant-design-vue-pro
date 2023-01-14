<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <editor
      api-key="cp4doryb5rrqrjh0bmz66u6xd8h3hibv5pzm2jibjk0cybpo"
      :init="{
        height: 500,
        menubar: false,
        plugins: [
          'a11ychecker','advlist','advcode','advtable','autolink','checklist','export',
          'lists','link','image','charmap','preview','anchor','searchreplace','visualblocks',
          'powerpaste','fullscreen','formatpainter','insertdatetime','media','table','help','wordcount'
        ],
        toolbar:
          'undo redo | casechange blocks | bold italic backcolor | \
          alignleft aligncenter alignright alignjustify | \
          bullist numlst checklist outdent indent | removeformat | a11ycheck code table help'
      }"
      initial-value="Welcome to TinyMCE Vue"
    />
  </div>
</template>

<script>

import Editor from '@tinymce/tinymce-vue'

export default {
name: 'TextEditor',
components: {
    'editor': Editor
}
}

</script>
