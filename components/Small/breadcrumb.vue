<template>
  <div class="flex mb-10">
    <div
      v-for="(item, index) in list"
      :key="index"
      class="flex items-center font-thin text-sm"
    >
      <p
        :class="{ 'text-[#EB3F36]': list.length === index + 1 }"
        class="capitalize"
        v-html="item"
      ></p>
      <svg
        v-if="list.length !== index + 1"
        width="13"
        height="13"
        viewBox="0 0 13 13"
        class="mt-1 mx-3"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M6.65865 3.40865C6.87018 3.19712 7.21315 3.19712 7.42468 3.40865L10.133 6.11698C10.3446 6.32852 10.3446 6.67148 10.133 6.88302L7.42468 9.59135C7.21315 9.80288 6.87018 9.80288 6.65865 9.59135C6.44712 9.37982 6.44712 9.03685 6.65865 8.82532L8.98397 6.5L6.65865 4.17468C6.44712 3.96315 6.44712 3.62018 6.65865 3.40865Z"
          fill="#868686"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M2.86702 3.40865C3.07856 3.19712 3.42152 3.19712 3.63306 3.40865L6.34139 6.11698C6.55292 6.32852 6.55292 6.67148 6.34139 6.88302L3.63306 9.59135C3.42152 9.80288 3.07856 9.80288 2.86702 9.59135C2.65549 9.37982 2.65549 9.03685 2.86702 8.82532L5.19234 6.5L2.86702 4.17468C2.65549 3.96315 2.65549 3.62018 2.86702 3.40865Z"
          fill="#868686"
        />
      </svg>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BreadcrumbComponents',
  props: ['list'],
}
</script>

<style></style>
