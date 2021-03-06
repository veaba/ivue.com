<template>
      <div>
            <h1>Button 按钮</h1>
            <p>按钮传达用户触摸它们时将发生的操作。它们可以是平坦的，凸起的，任何色彩辅助类都可以用来改变背景或文字的颜色。</p>
            <h2>基本用法</h2>
            <p>基本用法，凸陷的按钮具有单击时增加的框阴影，这是默认样式。</p>
            <DocMarkdown
                  :code="code.base"
                  jsfiddle="//jsfiddle.net/qq282126990/jw1ofmqk/"
                  github="//github.com/qq282126990/ivue.com/blob/master/src/views/components/button/Default.vue"
            >
                  <Default slot="demo"></Default>
            </DocMarkdown>
            <h2>平面</h2>
            <p>
                  通过设置属性
                  <code>flat</code> 使按钮没有框阴影，也没有背景。仅在悬停时显示按钮的背景。
            </p>
            <DocMarkdown
                  :code="code.flat"
                  jsfiddle="//jsfiddle.net/qq282126990/kwhoceqr/"
                  github="//github.com/qq282126990/ivue.com/blob/master/src/views/components/button/Flat.vue"
            >
                  <Flat slot="demo"></Flat>
            </DocMarkdown>
            <h2>凹陷</h2>
            <p>
                  通过设置属性
                  <code>depressed</code> 使按钮仍然保持其背景颜色，但没有框阴影。
            </p>
            <DocMarkdown
                  :code="code.depressed"
                  jsfiddle="//jsfiddle.net/qq282126990/jax7510u/"
                  github="//github.com/qq282126990/ivue.com/blob/master/src/views/components/button/Depressed.vue"
            >
                  <Depressed slot="demo"></Depressed>
            </DocMarkdown>
            <h2>轮廓</h2>
            <p>
                  通过设置属性
                  <code>outline</code> 使按钮继承其当前边框颜色。
            </p>
            <DocMarkdown
                  :code="code.outline"
                  jsfiddle="//jsfiddle.net/qq282126990/7ek59mfx/"
                  github="//github.com/qq282126990/ivue.com/blob/master/src/views/components/button/Outline.vue"
            >
                  <Outline slot="demo"></Outline>
            </DocMarkdown>
            <h2>链接</h2>
            <p>
                  通过设置属性
                  <code>href</code> 使按钮变成一个
                  <code>a</code>连接跳转到
                  <code>href</code>指定的地址。
            </p>
            <DocMarkdown
                  :code="code.href"
                  jsfiddle="//jsfiddle.net/qq282126990/L4waq3jo/"
                  github="//github.com/qq282126990/ivue.com/blob/master/src/views/components/button/Href.vue"
            >
                  <Href slot="demo"></Href>
            </DocMarkdown>
            <h2>图标</h2>
            <p>
                  通过设置属性
                  <code>icon</code> 使按钮显示为圆形图标。
            </p>
            <DocMarkdown
                  :code="code.icon"
                  jsfiddle="//jsfiddle.net/qq282126990/zw2hfn10/"
                  github="//github.com/qq282126990/ivue.com/blob/master/src/views/components/button/Icon.vue"
            >
                  <Icon slot="demo"></Icon>
            </DocMarkdown>
            <h2>API</h2>
            <h3>props</h3>
            <div class="table">
                  <table>
                        <thead>
                              <tr>
                                    <th>名称</th>
                                    <th>说明</th>
                                    <th>类型</th>
                                    <th>默认</th>
                              </tr>
                        </thead>
                        <tbody>
                              <tr>
                                    <td>href</td>
                                    <td>
                                          在按钮上创建一个锚点。在这种情况下，生成的标签将是
                                          <code>&lt;a&gt;</code>
                                    </td>
                                    <td>String</td>
                                    <td>null</td>
                              </tr>
                              <tr>
                                    <td>type</td>
                                    <td>将 type 应用于按钮 - 它不会影响链接</td>
                                    <td>String</td>
                                    <td>button</td>
                              </tr>
                              <tr>
                                    <td>disabled</td>
                                    <td>禁用该按钮并阻止其操作</td>
                                    <td>Boolean</td>
                                    <td>false</td>
                              </tr>
                              <tr>
                                    <td>ivue-ripple</td>
                                    <td>启用/禁用涟漪效应</td>
                                    <td>Boolean</td>
                                    <td>false</td>
                              </tr>
                              <tr>
                                    <td>color</td>
                                    <td>定义按钮颜色</td>
                                    <td>String</td>
                                    <td>null</td>
                              </tr>
                              <tr>
                                    <td>flat</td>
                                    <td>是否扁平按钮</td>
                                    <td>Boolean</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>depressed</td>
                                    <td>凹陷的按钮依然保持其背景色，但没有框阴影</td>
                                    <td>Boolean</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>icon</td>
                                    <td>按钮显示为圆形图标</td>
                                    <td>Boolean</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>outline</td>
                                    <td>轮廓按钮从当前色彩应用继承他们的边框颜色</td>
                                    <td>Boolean</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>to</td>
                                    <td>router-link</td>
                                    <td>String,Object</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>replace</td>
                                    <td>router-link</td>
                                    <td>Boolean</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>append</td>
                                    <td>router-link</td>
                                    <td>Boolean</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>tag</td>
                                    <td>router-link</td>
                                    <td>String</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>active-class</td>
                                    <td>router-link</td>
                                    <td>String</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>exact</td>
                                    <td>router-link</td>
                                    <td>Boolean</td>
                                    <td>undefined</td>
                              </tr>
                              <tr>
                                    <td>event</td>
                                    <td>router-link</td>
                                    <td>String, Array</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>exact-active-class</td>
                                    <td>router-link</td>
                                    <td>String</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>href</td>
                                    <td>router-link</td>
                                    <td>String, Object</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>disabled</td>
                                    <td>router-link</td>
                                    <td>Boolean</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>nuxt</td>
                                    <td>router-link</td>
                                    <td>Boolean</td>
                                    <td>-</td>
                              </tr>
                              <tr>
                                    <td>target</td>
                                    <td>router-link</td>
                                    <td>String</td>
                                    <td>-</td>
                              </tr>
                        </tbody>
                  </table>
            </div>
            <h3>event</h3>
            <div class="table">
                  <table>
                        <thead>
                              <tr>
                                    <th>名称</th>
                                    <th>说明</th>
                              </tr>
                        </thead>
                        <tbody>
                              <tr>
                                    <td>click</td>
                                    <td>单击鼠标后触发</td>
                              </tr>
                        </tbody>
                  </table>
            </div>
            <h3>slot</h3>
            <div class="table">
                  <table>
                        <thead>
                              <tr>
                                    <th>名称</th>
                                    <th>说明</th>
                              </tr>
                        </thead>
                        <tbody>
                              <tr>
                                    <td>ivue-icon</td>
                                    <td>添加图标</td>
                              </tr>
                        </tbody>
                  </table>
            </div>
      </div>
</template>

<script>
import DocMarkdown from '@/components/DocMarkdown';
import Code from '@/code/button';

import Default from './components/button/Default.vue';
import Flat from './components/button/Flat.vue';
import Depressed from './components/button/Depressed.vue';
import Outline from './components/button/Outline.vue';
import Href from './components/button/Href.vue';
import Icon from './components/button/Icon.vue';

export default {
      name: 'ivue-button',
      data () {
            return {
                  code: Code
            }
      },
      components: {
            DocMarkdown,
            Default,
            Flat,
            Depressed,
            Outline,
            Href,
            Icon
      }
}
</script>

<style lang="scss" scope>
</style>
