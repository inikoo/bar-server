<!--
  - Author: Raul Perusquia <raul@inikoo.com>
  - Created: Mon, 24 Jul 2023 12:11:04 Malaysia Time, Kuala Lumpur, Malaysia
  - Copyright (c) 2023, Raul A Perusquia Flores
  -->

<script setup lang="ts">

const props = defineProps<{
    data: {
        label?:string
        target:string
    }
    }>()

</script>

<template>
    <Link  :href="data.target"
          class="bg-gray-800/40 text-gray-100 border border-gray-50/50 absolute bottom-6 right-11 rounded-md px-3 py-1 hover:bg-gray-900/60 whitespace-nowrap">
        {{ data.label?.length == 0 ? trans('Open') : data.label }}
    </Link>
</template>
