<template>
    <div class="kl-content">
        <h2 class="kl-content__title">按钮<span>KLButton</span></h2>
        <div class="kl-content__demo">
            <Demo title="按钮类型">
                <div slot="desc">
                    <p>主按钮、次按钮、弱按钮及不可点4种状态，主按钮在同一操作区只能出现一个</p>
                    <p>通过设置<code>type</code>为<code>primary</code>、<code>ghost</code>、<code>dashed</code>、<code>text</code>、<code>info</code>、<code>success</code>、<code>warning</code>、<code>error</code>创建不同样式的按钮，不设置为默认样式。</p>
                </div>
                <div slot="demo">
                    <button class="kl-btn" :class="$style['kl-primary']">主按钮</button>
                    <button class="kl-btn" :class="$style['kl-secondary']">次按钮</button>
                    <button class="kl-btn">弱按钮</button>
                    <button disabled="disabled" class="kl-btn" :class="$style['kl-disabled']">不可点</button>
                </div>
                <div slot="code">
                    <i-code lang="html" slot="code">{{ code.icon }}</i-code>
                </div>
            </Demo>
            <Demo title="按钮类型">
                <div slot="demo">
                    <button>Default</button>
                </div>
                <div slot="desc">
                    <p>按钮类型有：默认按钮、主按钮、幽灵按钮、虚线按钮、文字按钮以及四种颜色按钮。</p>
                    <p>通过设置<code>type</code>为<code>primary</code>、<code>ghost</code>、<code>dashed</code>、<code>text</code>、<code>info</code>、<code>success</code>、<code>warning</code>、<code>error</code>创建不同样式的按钮，不设置为默认样式。</p>
                </div>
                <hr>
                <i-code lang="html" slot="code">{{ code.icon }}</i-code>
            </Demo>
            <Demo title="按钮类型">
                <div slot="demo">
                    <button>Default</button>
                </div>
                <div slot="desc">
                    <p>按钮类型有：默认按钮、主按钮、幽灵按钮、虚线按钮、文字按钮以及四种颜色按钮。</p>
                    <p>通过设置<code>type</code>为<code>primary</code>、<code>ghost</code>、<code>dashed</code>、<code>text</code>、<code>info</code>、<code>success</code>、<code>warning</code>、<code>error</code>创建不同样式的按钮，不设置为默认样式。</p>
                </div>
                <hr>
                <i-code lang="html" slot="code">{{ code.icon }}</i-code>
            </Demo>
            <Demo title="按钮类型">
                <div slot="demo">
                    <button>Default</button>
                </div>
                <div slot="desc">
                    <p>按钮类型有：默认按钮、主按钮、幽灵按钮、虚线按钮、文字按钮以及四种颜色按钮。</p>
                    <p>通过设置<code>type</code>为<code>primary</code>、<code>ghost</code>、<code>dashed</code>、<code>text</code>、<code>info</code>、<code>success</code>、<code>warning</code>、<code>error</code>创建不同样式的按钮，不设置为默认样式。</p>
                </div>
                <hr>
                <i-code lang="html" slot="code">{{ code.icon }}</i-code>
            </Demo>
        </div>
        <div class="kl-content__table">
            <h1>
                <a href="#API" class="headerlink" title="API"></a>API
            </h1>
        </div>
    </div>
</template>
<script>
import iCode from 'iCode';
import Demo from '../../components/demo.vue';
import Code from '../../code/button';
export default {
    components: {
        iCode,
        Demo
    },
    name: 'KLbutton',
    data () {
        return {
           code: Code
        }
    },
    methods: {

    }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style module>
@component-namespace kl {
    @b primary {
        color: #fff;
        background: #e31436;
        border: 1px solid #e31436;
    }
    @b secondary {
        color: #e31436;
        background: #fff;
        border: 1px solid #e31436;
    }
    @b disabled {
        cursor: not-allowed;
        filter: alpha(opacity = 50);
        opacity: 0.5;
        -webkit-box-shadow: none;
        box-shadow: none;
    }    
}
</style>