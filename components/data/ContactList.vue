<template>
  <div>
    <!--  -->
    <div>
      <p>Company: <span>All</span></p>
    </div>
    <!--  -->
    <div class="flex flex-col">
      <div class="-my-2 overflow-x-auto sm:-mx-6 lg:-mx-8">
        <div class="py-2 align-middle inline-block min-w-full sm:px-6 lg:px-8">
          <div
            class="shadow overflow-hidden border-b border-gray-200 sm:rounded-lg"
          >
            <table class="min-w-full divide-y divide-gray-200">
              <thead class="bg-white">
                <tr>
                  <th scope="col" class="py-3 px-2">
                    <label class="inline-flex items-center">
                      <input
                        type="checkbox"
                        class="form-checkbox text-green-500"
                      />
                    </label>
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Name
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Email
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Company Name
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Role
                  </th>
                  <th
                    scope="col"
                    class="px-6 py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Forecast
                  </th>
                  <th
                    scope="col"
                    class="py-3 text-left text-xs font-medium text-gray-500 uppercase tracking-wider"
                  >
                    Recent Activity
                  </th>
                </tr>
              </thead>
              <Contact
                v-for="(contact, index) in contacts"
                :key="index"
                :contact="contact"
              />
              <!--  -->
            </table>
          </div>
        </div>
      </div>
    </div>

    <!--  -->
  </div>
</template>

<script>
import Contact from "~/components/data/Contact";
export default {
  props: {
    contacts: {
      type: Array,
      required: true
    }
  },
  components: {
    Contact
  }
};
</script>
