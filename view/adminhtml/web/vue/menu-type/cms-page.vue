<template>
    <auto-complete
        :label="config.translation.page"
        :description="config.translation.pageId"
        :item="item"
        item-key="content"
        :options="config.fieldData.cms_page.snowMenuAutoCompleteField.options"
        :config="config"
    />
</template>

<script>
    define(['Vue'], function(Vue) {
        Vue.component('cms_page', {
            props: {
                config: {
                    type: Object,
                    required: true
                },
                item: {
                    type: Object,
                    required: true
                }
            },
            template: template
        });
    });
</script>
