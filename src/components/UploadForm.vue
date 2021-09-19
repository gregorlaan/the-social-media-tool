<template>
  <div>
    <div class="container bg-gray-100 p-4 rounded-lg">
      <div class="row">
        <div class="col-12 mb-4">
          <label>Image</label>

          <label
            for="file"
            class="block cursor-pointer text-center p-10 border border-dashed rounded-lg border-gray-300 bg-white"
          >
            Drag your files here or click in this area.
          </label>

          <input
            id="file"
            type="file"
            name="file"
            multiple
            class="w-0 h-0 hidden"
          >
        </div>

        <div class="col-12 mb-4">
          <div class="flex flex-col space-y-2">
            <label
              for="default"
              class="text-gray-700 select-none font-medium"
            >
              Title
            </label>

            <input
              id="title"
              v-model="title"
              name="title"
              type="text"
              placeholder="Title"
              class="px-4 py-2 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-gray-200"
            >
          </div>
        </div>

        <div class="col-12 mb-4">
          <div class="flex flex-col space-y-2">
            <label
              for="default"
              class="text-gray-700 select-none font-medium"
            >
              Description
            </label>

            <input
              id="description"
              v-model="description"
              name="description"
              type="text"
              placeholder="Description"
              class="px-4 py-2 rounded-lg border border-gray-300 focus:outline-none focus:ring-2 focus:ring-gray-200"
            >
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap-grid.min.css';

export default {
  name: 'UploadForm',

  components: {
  },

  data() {
    return {
      description: '',
      title: '',
    };
  },

  methods: {
    onUpload: function () {},
  },
};
</script>

<style scoped>
</style>
