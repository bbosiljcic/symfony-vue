<template>
    <div class="container-fluid">
        <div class="row">
            <aside class="col-xs-12 col-3">
                <div class="sidebar p-3 mb-5">
                    <h5 class="text-center">
                        Categories
                    </h5>

                    <ul class="nav flex-column mb4">
                        <li class="nav-item">
                            <a
                                class="nav-link"
                                href="/"
                            >All Products</a>
                        </li>
                        <li class="nav-item">
                            <a
                                class="nav-link"
                                href="#"
                            >Category A</a>
                        </li>
                        <li class="nav-item">
                            <a
                                class="nav-link"
                                href="#"
                            >Category B</a>
                        </li>
                    </ul>
                </div>
            </aside>

            <div class="col-xs-12 col-9">
                <div class="row">
                    <div class="col-12">
                        <h1>
                            Products
                        </h1>
                    </div>
                </div>

                <div class="row">
                    <div class="col-xs-12 col-6 mb-2 pb-2">
                        TODO - load some products!
                    </div>
                </div>

                <div class="row">
                    <base-legend :title="legend" />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import BaseLegend from '../Components/BaseLegend';

export default {
    name: 'ProductsPage',
    components: {
        BaseLegend,
    },
    data() {
        return {
            legend: 'Dynamic legend',
        };
    },
};
</script>

<style lang="scss" scoped>
@import '../../scss/components/light-component';
.sidebar {
    @include light-component;

    ul {
        li a:hover {
            background: $blue-component-link-hover;
        }
    }
}
</style>
