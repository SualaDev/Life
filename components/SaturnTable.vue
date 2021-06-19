<template>
  <div v-if="data !== null" class="table-ctn">
    <div class="table-header">
      {{ data.title }}
    </div>
    <table :class="['table', (data.styles.fullWidth ? 'full-width' : '')]">
      <tr class="header-row">
        <th>
          <button class="clear-btn checkbox">
            <svg
              class="unchecked"
              width="20"
              height="20"
              viewBox="0 0 20 20"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path d="M19 0H1C0.734784 0 0.48043 0.105357 0.292893 0.292893C0.105357 0.48043 0 0.734784 0 1V19C0 19.2652 0.105357 19.5196 0.292893 19.7071C0.48043 19.8946 0.734784 20 1 20H19C19.2652 20 19.5196 19.8946 19.7071 19.7071C19.8946 19.5196 20 19.2652 20 19V1C20 0.734784 19.8946 0.48043 19.7071 0.292893C19.5196 0.105357 19.2652 0 19 0ZM18 18H2V2H18V18Z" fill="#7C86A1" />
            </svg>
            <svg
              class="checked"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path d="M10.21 14.75C10.303 14.8437 10.4136 14.9181 10.5354 14.9689C10.6573 15.0197 10.788 15.0458 10.92 15.0458C11.052 15.0458 11.1827 15.0197 11.3046 14.9689C11.4264 14.9181 11.537 14.8437 11.63 14.75L15.71 10.67C15.8983 10.4817 16.0041 10.2263 16.0041 9.96C16.0041 9.6937 15.8983 9.4383 15.71 9.25C15.5217 9.0617 15.2663 8.95591 15 8.95591C14.7337 8.95591 14.4783 9.0617 14.29 9.25L10.92 12.63L9.71 11.41C9.5217 11.2217 9.2663 11.1159 9 11.1159C8.7337 11.1159 8.4783 11.2217 8.29 11.41C8.1017 11.5983 7.99591 11.8537 7.99591 12.12C7.99591 12.3863 8.1017 12.6417 8.29 12.83L10.21 14.75ZM21 2H3C2.73478 2 2.48043 2.10536 2.29289 2.29289C2.10536 2.48043 2 2.73478 2 3V21C2 21.2652 2.10536 21.5196 2.29289 21.7071C2.48043 21.8946 2.73478 22 3 22H21C21.2652 22 21.5196 21.8946 21.7071 21.7071C21.8946 21.5196 22 21.2652 22 21V3C22 2.73478 21.8946 2.48043 21.7071 2.29289C21.5196 2.10536 21.2652 2 21 2ZM20 20H4V4H20V20Z" fill="#FF691C" />
            </svg>
          </button>
        </th>
        <th v-for="(header) in data.headers" :key="header.key">
          {{ header.label }}
        </th>
        <th>
          Action
        </th>
      </tr>
      <tr v-for="(label, index) in data.labels" :key="index">
        <td>
          <button class="clear-btn checkbox">
            <svg
              class="unchecked"
              width="20"
              height="20"
              viewBox="0 0 20 20"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path d="M19 0H1C0.734784 0 0.48043 0.105357 0.292893 0.292893C0.105357 0.48043 0 0.734784 0 1V19C0 19.2652 0.105357 19.5196 0.292893 19.7071C0.48043 19.8946 0.734784 20 1 20H19C19.2652 20 19.5196 19.8946 19.7071 19.7071C19.8946 19.5196 20 19.2652 20 19V1C20 0.734784 19.8946 0.48043 19.7071 0.292893C19.5196 0.105357 19.2652 0 19 0ZM18 18H2V2H18V18Z" fill="#7C86A1" />
            </svg>
            <svg
              class="checked"
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path d="M10.21 14.75C10.303 14.8437 10.4136 14.9181 10.5354 14.9689C10.6573 15.0197 10.788 15.0458 10.92 15.0458C11.052 15.0458 11.1827 15.0197 11.3046 14.9689C11.4264 14.9181 11.537 14.8437 11.63 14.75L15.71 10.67C15.8983 10.4817 16.0041 10.2263 16.0041 9.96C16.0041 9.6937 15.8983 9.4383 15.71 9.25C15.5217 9.0617 15.2663 8.95591 15 8.95591C14.7337 8.95591 14.4783 9.0617 14.29 9.25L10.92 12.63L9.71 11.41C9.5217 11.2217 9.2663 11.1159 9 11.1159C8.7337 11.1159 8.4783 11.2217 8.29 11.41C8.1017 11.5983 7.99591 11.8537 7.99591 12.12C7.99591 12.3863 8.1017 12.6417 8.29 12.83L10.21 14.75ZM21 2H3C2.73478 2 2.48043 2.10536 2.29289 2.29289C2.10536 2.48043 2 2.73478 2 3V21C2 21.2652 2.10536 21.5196 2.29289 21.7071C2.48043 21.8946 2.73478 22 3 22H21C21.2652 22 21.5196 21.8946 21.7071 21.7071C21.8946 21.5196 22 21.2652 22 21V3C22 2.73478 21.8946 2.48043 21.7071 2.29289C21.5196 2.10536 21.2652 2 21 2ZM20 20H4V4H20V20Z" fill="#FF691C" />
            </svg>
          </button>
        </td>
        <td v-for="(header) in data.headers" :key="header.key">
          <!--
            Information here renders based on the type of the [label]
            Valid types are 'date/time', 'currency'
          -->
          {{ formatCell(header.type, label[header.key]) }}
        </td>
        <td class="action">
          <button class="clear-btn" @click="$emit('action')">
            <svg
              v-if="data.styles.actionText === undefined"
              width="24"
              height="24"
              viewBox="0 0 16 16"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path opacity="0.4" d="M8.00016 1.33366C11.6768 1.33366 14.6668 4.32433 14.6668 8.00033C14.6668 11.6763 11.6768 14.667 8.00016 14.667C4.32416 14.667 1.3335 11.6763 1.3335 8.00033C1.3335 4.32433 4.32416 1.33366 8.00016 1.33366Z" fill="#75759E" />
              <path d="M7.03865 5.18693C7.16598 5.18693 7.29398 5.2356 7.39131 5.33293L9.71598 7.64626C9.80998 7.74026 9.86265 7.8676 9.86265 8.00093C9.86265 8.1336 9.80998 8.26093 9.71598 8.35493L7.39131 10.6696C7.19598 10.8643 6.87998 10.8643 6.68465 10.6683C6.48998 10.4723 6.49065 10.1556 6.68598 9.96093L8.65465 8.00093L6.68598 6.04093C6.49065 5.84626 6.48998 5.53026 6.68465 5.33426C6.78198 5.2356 6.91065 5.18693 7.03865 5.18693Z" fill="#75759E" />
            </svg>
            <span type="button" class="link">
              {{ data.styles.actionText }}
            </span>
          </button>
        </td>
      </tr>
    </table>
    <div class="pagination">
      ---pagination---
    </div>
  </div>
  <div v-else class="stuff">
    Add Data to mount table
  </div>
</template>

<script>
export default {
  name: 'SaturnTable',
  props: {
    /**
     * @name data
     * @type {Object}
     * @returns Encapsulated Data of to be rendered by DOM table
     *  @name data.title is the main title of the Table, must have a type of String
     *  @name data.headers are the contents of each column in the table, must have a type of Array<Object>
     *  @name data.labels are the contents in each cell respective to the headers initially defined, must have a type of Array<Object>
     *  @name data.styles are used to manipulate the default look of the table, must have a type of Object
     *   @name data.styles.fullWidth boolean value to apply a full width to the table's vertical edges, defaults to false
     *   @name data.styles.actionText string value to replace the action icon, if [actionText] is undefined, icon is used
     */
    data: {
      type: Object,
      default: null
    }
  },
  created () {
    this.$emit('created')
  },
  mounted () {
    this.$emit('mounted')
  },
  methods: {
    formatDate (dateString) {
      const date = new Date(dateString)
      const dayString = date.toLocaleDateString()
      const timeString = date.toLocaleTimeString()
      return `${dayString},  ${timeString}`
    },
    formatCurrency (num) {
      return '₦' + num.toString().replace(/(\d)(?=(\d{3})+(?!\d))/g, '$1,')
    },
    /**
     * @type {String}
     * @returns formatted and more accurate string based on the type assigned in {data.headers[i].key}
     *  valid keys are 'date/time', 'currency'
     */
    formatCell (type, rawContent) {
      if (type === 'date/time') {
        return this.formatDate(rawContent)
      } else if (type === 'currency') {
        return this.formatCurrency(rawContent)
      } else {
        return rawContent
      }
    }
  }
}
</script>

<style scoped>
/* Global Styles */
.clear-btn {
  width: 100%;
  text-align: left;
  border: none;
  background: transparent;
  cursor: pointer;
}
.clear-btn.checkbox {
  display: grid;
  place-items: center;
}
.link {
  text-decoration: underline;
  text-align: left;
  height: 24px;
}

.table {
  margin: 24px 0;
  border-spacing: 0px;
  overflow-x: auto;
  border: 1px solid #E2E2EA;
  border-radius: 20px;
}
.full-width {
  width: 100%;
}
.header-row {
  text-align: left;
  background: #F0F2F4;
  border-radius: 20px 20px 0px 0px;
  font-size: 16px;
  line-height: 18px;
}
th {
  color: #75759E;
}
th {
  padding: 24px 14px;
  white-space: nowrap;
}
td {
  padding: 18px 14px;
  white-space: nowrap;
}
</style>
