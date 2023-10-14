<script>
</script>

<template>
    <div>
        <div>
            <h2>EvoMarket</h2>
        </div>
        <div>
            <i class="fa-sharp fa-regular fa-location-dot"></i>
        </div>
        <div>
            <template>
                <el-row class="demo-autocomplete">
                    <el-col :span="12">
                        <div class="sub-title my-2 text-sm text-gray-600">
                            list suggestions when activated
                        </div>
                        <el-autocomplete v-model="state1" :fetch-suggestions="querySearch" clearable
                            class="inline-input w-50" placeholder="Please Input" @select="handleSelect" />
                    </el-col>
                    <el-col :span="12">
                        <div class="sub-title my-2 text-sm text-gray-600">
                            list suggestions on input
                        </div>
                        <el-autocomplete v-model="state2" :fetch-suggestions="querySearch" :trigger-on-focus="false"
                            clearable class="inline-input w-50" placeholder="Please Input" @select="handleSelect" />
                    </el-col>
                </el-row>
            </template>
        </div>
        <div>

        </div>

    </div>
</template>

<style></style>