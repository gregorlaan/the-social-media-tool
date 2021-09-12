<template>
  <div>
    <FileUpload
      name="image[]"
      :multiple="false"
      accept="image/*"
      :max-file-size="1000000"
      @upload="onUpload"
    >
      <template #empty>
        <p>Drag and drop files to here to upload.</p>
      </template>
    </FileUpload>

    <Textarea
      v-model="caption"
      :auto-resize="true"
      placeholder="Caption"
      rows="5"
      cols="100"
    />
  </div>
</template>

<script>
import Textarea from "primevue/textarea";
import FileUpload from "primevue/fileupload";

export default {
  name: "UploadForm",

  components: {
    Textarea,
    FileUpload,
  },

  data() {
    return {
      caption: "",
    };
  },

  methods: {
    onUpload: function () {},
  },
};
</script>

<style scoped>
</style>
