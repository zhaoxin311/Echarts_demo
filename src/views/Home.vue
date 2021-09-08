<template>
  <div class="home">
    <div class="app-wrap">
      <div class="website-warp">
        <div style="padding: 0 20px">
          <el-row>
            <el-col :span="6" class="website">
              <div class="logo">
                <svg
                  width="47"
                  height="47"
                  viewBox="0 0 47 47"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <rect
                    width="47"
                    height="47"
                    rx="4"
                    fill="#0A6CF2"
                    fill-opacity="0.1"
                  />
                  <g clip-path="url(#clip0)">
                    <path
                      d="M37.2476 28.8993C36.8975 28.5308 31.205 23.5383 30.8365 23.1883C30.6601 22.9789 30.4089 22.8467 30.1365 22.8198H21.0541C21.0541 22.8198 19.6356 23.0041 19.6356 24.2568C19.6123 25.1294 20.2045 25.8986 21.0541 26.099C21.9568 26.2648 23.5412 26.6333 24.9781 26.7991C25.5124 26.7991 24.9781 27.1676 24.9781 27.1676L23.1359 28.4019H17.1486C17.1486 28.4019 14.6615 26.6517 12.8745 25.1411C10.2217 23.1883 9.19 25.1411 9.19 25.1411C9.19 25.1411 8.82155 25.8596 9.19 26.2096C10.6085 27.4623 15.7669 32.1048 16.1169 32.4548C16.3575 32.6699 16.6947 32.7401 17.0012 32.6391H27.502C28.0246 32.6361 28.5298 32.8264 28.9206 33.1733C28.9206 33.1733 30.5233 34.6103 31.0576 35.0156C31.9419 35.734 32.3103 35.0156 32.3103 35.0156L37.1002 29.8388C37.265 29.7674 37.3849 29.6203 37.4215 29.4444C37.4581 29.2686 37.407 29.0859 37.2844 28.9545L37.2476 28.8993ZM25.7335 13.8665H12.1376C11.6989 13.7783 11.3832 13.3929 11.3832 12.9453C11.3832 12.4978 11.6989 12.1124 12.1376 12.0242H25.7335C26.1065 11.9492 26.4879 12.1066 26.6995 12.4228C26.9111 12.739 26.9111 13.1516 26.6995 13.4678C26.4879 13.784 26.1065 13.9414 25.7335 13.8665ZM25.7335 19.1722H12.1376C11.6289 19.1722 11.2165 18.7598 11.2165 18.251C11.2165 17.7423 11.6289 17.3299 12.1376 17.3299H25.7335C26.2422 17.3299 26.6546 17.7423 26.6546 18.251C26.6546 18.7598 26.2422 19.1722 25.7335 19.1722Z"
                      fill="#0A6CF2"
                    />
                  </g>
                  <defs>
                    <clipPath id="clip0">
                      <rect
                        width="28.4444"
                        height="23.7037"
                        fill="white"
                        transform="translate(9 12)"
                      />
                    </clipPath>
                  </defs>
                </svg>
              </div>
              <div class="left">
                <div class="title-top">出让方数量</div>
                <div class="title-num">{{ showtransferorNumber }}</div>
              </div>
              <div ref="website_transferor" class="website-style" />
              <div class="foot">占比：{{ transferorPercent * 100 }}%</div>
            </el-col>
            <el-col :span="6" class="website">
              <div class="logo">
                <svg
                  width="47"
                  height="47"
                  viewBox="0 0 47 47"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <rect
                    width="47"
                    height="47"
                    rx="4"
                    fill="#F2900A"
                    fill-opacity="0.1"
                  />
                  <path
                    d="M8.74577 28.9132C9.09621 28.5444 14.7954 23.546 15.1643 23.1956C15.3409 22.986 15.5924 22.8536 15.8652 22.8267H24.9581C24.9581 22.8267 26.3783 23.0111 26.3783 24.2653C26.4016 25.139 25.8087 25.909 24.9581 26.1097C24.0543 26.2757 22.4681 26.6446 21.0295 26.8106C20.4946 26.8106 21.0295 27.1795 21.0295 27.1795L22.8739 28.4152H28.8682C28.8682 28.4152 31.3582 26.6631 33.1472 25.1506C35.8032 23.1956 36.8361 25.1506 36.8361 25.1506C36.8361 25.1506 37.2049 25.87 36.8361 26.2204C35.4159 27.4746 30.2515 32.1225 29.9011 32.4729C29.6602 32.6883 29.3226 32.7586 29.0158 32.6574H18.5027C17.9795 32.6544 17.4737 32.8449 17.0825 33.1923C17.0825 33.1923 15.4779 34.6309 14.943 35.0367C14.0577 35.756 13.6888 35.0367 13.6888 35.0367L8.89333 29.8539C8.7283 29.7824 8.60832 29.6351 8.57164 29.459C8.53496 29.283 8.58614 29.1 8.70889 28.9686L8.74577 28.9132ZM20.2733 13.8629H33.885C34.3243 13.7746 34.6403 13.3887 34.6403 12.9407C34.6403 12.4926 34.3243 12.1068 33.885 12.0185H20.2733C19.8999 11.9434 19.518 12.101 19.3062 12.4176C19.0943 12.7341 19.0943 13.1472 19.3062 13.4638C19.518 13.7804 19.8999 13.938 20.2733 13.8629ZM20.2733 19.1748H33.885C34.3943 19.1748 34.8072 18.7619 34.8072 18.2526C34.8072 17.7433 34.3943 17.3304 33.885 17.3304H20.2733C19.764 17.3304 19.3511 17.7433 19.3511 18.2526C19.3511 18.7619 19.764 19.1748 20.2733 19.1748Z"
                    fill="#F2900A"
                  />
                </svg>
              </div>
              <div class="left">
                <div class="title-top">受让方数量</div>
                <div class="title-num">{{ showtransfereeNumber }}</div>
              </div>
              <div ref="website_assignee" class="website-style" />
              <div class="foot">占比：{{ transfereePercent * 100 }}%</div>
            </el-col>
            <el-col :span="6" class="website">
              <div class="logo">
                <svg
                  width="47"
                  height="47"
                  viewBox="0 0 47 47"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <rect
                    width="47"
                    height="47"
                    rx="4"
                    fill="#0FA465"
                    fill-opacity="0.1"
                  />
                  <path
                    d="M25.2066 32.4512C25.7223 32.1781 25.9301 31.5484 25.6547 31.0293C25.6547 31.0293 25.1416 30.0652 24.8591 29.5412C24.7151 30.2193 24.3188 30.4475 23.3838 31.2571L23.7884 32.0187C23.9717 32.361 24.6826 32.7323 25.2066 32.4512ZM22.4911 31.2261L23.9301 29.9798C24.4133 29.5567 24.3891 28.8363 23.9751 28.4366C23.5761 28.0316 22.9418 28.0362 22.5467 28.3811L21.1073 29.6311C20.6638 30.0142 20.6279 30.6802 21.0087 31.1203C21.3401 31.4981 22.0027 31.6432 22.4911 31.2261ZM27.5447 31.2129C28.0936 30.919 28.2504 30.2836 27.9935 29.7868L26.3656 26.7472L26.8284 26.4559L28.6391 29.8733C28.9092 30.3822 29.5363 30.5756 30.0573 30.3096C30.5994 30.0172 30.7724 29.3871 30.5053 28.8839L28.6229 25.3388L29.1023 25.0513C29.1023 25.0513 30.3474 27.4476 30.7958 28.3014C31.0731 28.8182 31.7146 29.0036 32.2148 28.7339C32.7406 28.4559 32.9371 27.8291 32.6624 27.3086C31.2526 24.6384 31.5589 25.2002 30.9843 24.2584C29.2874 21.9018 26.8133 20.2842 24.377 18.2664L20.0473 20.2996C19.1531 20.7107 18.2121 20.283 17.8411 19.5176C17.4361 18.6744 17.7927 17.6915 18.6129 17.2944L19.6487 16.8082L16.3213 16.7988L12.7962 21.6226L15.0935 23.7352C15.1902 23.5225 15.3334 23.3317 15.5121 23.1764L18.0915 20.9366C18.7791 20.3491 19.8203 20.4088 20.4292 21.102C20.7296 21.4519 20.8727 21.8818 20.8384 22.3245C21.4402 22.1885 22.0518 22.4039 22.4462 22.8542C22.9297 23.4118 22.9917 24.1957 22.6215 24.8012C23.0072 24.8636 23.354 25.0559 23.6082 25.3494C24.1757 26.0064 24.1451 26.9546 23.5916 27.5594C23.9709 27.5035 24.4193 27.7041 24.6305 28.029C24.6305 28.029 25.7283 30.0229 26.1273 30.7792C26.3071 31.1226 27.023 31.4917 27.5447 31.2129ZM20.7571 29.2277L23.054 27.2364C23.4858 26.865 23.5402 26.2005 23.1477 25.7476C22.7756 25.3146 22.1103 25.258 21.6699 25.6426C21.6162 25.6894 19.3412 27.6588 19.2917 27.7105C18.9264 28.1019 18.9208 28.709 19.2793 29.123C19.6189 29.5167 20.2898 29.6334 20.7571 29.2277ZM18.7398 27.474L21.8905 24.7431C22.3287 24.3676 22.3778 23.7034 21.9887 23.2542C21.6011 22.8119 20.9434 22.7714 20.5105 23.1485L17.6337 25.6376C16.9669 26.0585 16.8751 26.9251 17.2623 27.3698C17.5842 27.7475 18.2627 27.8915 18.7398 27.474ZM15.8143 25.125C15.4233 24.6728 15.48 24.0068 15.9087 23.6362L18.489 21.396C18.9211 21.0272 19.5857 21.0609 19.9714 21.5017C20.3586 21.9524 20.3174 22.6071 19.8769 22.9906L17.2929 25.2308C16.8887 25.5848 16.2257 25.595 15.8143 25.125ZM24.4684 17.5521L19.7881 19.7488C19.2373 20.0061 18.6303 19.7538 18.387 19.2528C18.1248 18.705 18.3639 18.09 18.8766 17.8403L23.5867 15.6311C24.2414 15.3923 24.8949 15.2846 25.6985 15.2846C27.3176 15.2846 30.6421 16.1562 32.1736 16.591L34.9246 21.2826L33.347 22.2769C32.9692 22.6392 32.6602 23.6607 31.8328 24.2044C30.1393 21.9094 27.1786 19.5169 24.4684 17.5521ZM32.5997 15.6307L35.492 13.8631L38.9709 19.682L35.965 21.368L32.5997 15.6307ZM8.85413 19.3424L12.9183 13.4316L15.908 15.8286L11.9375 21.3374L8.85413 19.3424Z"
                    fill="#0FA465"
                  />
                </svg>
              </div>
              <div class="left">
                <div class="title-top">中介机构量</div>
                <div class="title-num">{{ showagencyNumber }}</div>
              </div>
              <div ref="website_proxy" class="website-style" />
              <div class="foot">占比：{{ agencyPercent * 100 }}%</div>
            </el-col>
            <el-col :span="6" class="website">
              <div class="logo">
                <svg
                  width="47"
                  height="47"
                  viewBox="0 0 47 47"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <rect
                    width="47"
                    height="47"
                    rx="4"
                    fill="#8794AE"
                    fill-opacity="0.1"
                  />
                  <path
                    d="M32 29C33.1 29 33.99 28.1 33.99 27L34 17C34 15.9 33.1 15 32 15H16C14.9 15 14 15.9 14 17V27C14 28.1 14.9 29 16 29H12V31H36V29H32ZM16 17H32V27H16V17Z"
                    fill="#8794AE"
                  />
                </svg>
              </div>
              <div class="left">
                <div class="title-top">网站用户数</div>
                <div class="title-num">{{ showvisitorNumber }}</div>
              </div>
              <div ref="website_user" class="website-style" />
              <div class="foot">占比：{{ visitorPercent * 100 }}%</div>
            </el-col>
          </el-row>
        </div>
      </div>
      <div class="business-warp">
        <div class="top">
          <div class="block">
            <span class="demonstration">时间选择</span>
            <el-date-picker
              v-model="value1"
              type="datetimerange"
              range-separator="至"
              start-placeholder="开始日期"
              end-placeholder="结束日期"
            />
          </div>
          <div class="radio">
            <el-radio-group v-model="radio">
              <el-radio :label="3">近7天</el-radio>
              <el-radio :label="6">近30天</el-radio>
            </el-radio-group>
          </div>
        </div>
        <div class="bottom">
          <el-row>
            <el-col :span="6" class="echarts">
              <div class="title-left" />
              <div class="title">代办业务量</div>
              <div class="title_number">130</div>
              <div ref="business_acting" class="echarts-style" />
              <div class="foot_echarts">
                <p style="margin: 0 0 0 20px; display: inline-block">同比</p>
                <svg
                  style="margin: -4px 0; display: inline-block"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M5.83334 11.6667L10 7.5L14.1667 11.6667H5.83334Z"
                    fill="#0FA465"
                  />
                </svg>
                <p style="display: inline-block; margin: 0">3</p>
                <p style="margin: 0 0 0 20px; display: inline-block">环比</p>
                <svg
                  style="margin: -4px 0; display: inline-block"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M5.83334 11.6667L10 7.5L14.1667 11.6667H5.83334Z"
                    fill="#EB1A09"
                  />
                </svg>
                <p style="display: inline-block; margin: 0">108</p>
              </div>
            </el-col>
            <el-col :span="6" class="echarts">
              <div class="title-left" />
              <div class="title">已结办业务量</div>
              <div class="title_number">429</div>
              <div ref="business_finish" class="echarts-style" />
              <div class="foot_echarts">
                <p style="margin: 0 0 0 20px; display: inline-block">同比</p>
                <svg
                  style="margin: -4px 0; display: inline-block"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M5.83334 11.6667L10 7.5L14.1667 11.6667H5.83334Z"
                    fill="#0FA465"
                  />
                </svg>
                <p style="display: inline-block; margin: 0">3</p>
                <p style="margin: 0 0 0 20px; display: inline-block">环比</p>
                <svg
                  style="margin: -4px 0; display: inline-block"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M5.83334 11.6667L10 7.5L14.1667 11.6667H5.83334Z"
                    fill="#EB1A09"
                  />
                </svg>
                <p style="display: inline-block; margin: 0">108</p>
              </div>
            </el-col>
            <el-col :span="6" class="echarts">
              <div class="title-left" />
              <div class="title">已办结份额业务量</div>
              <div class="title_number">583</div>
              <div ref="business_share" class="echarts-style" />
              <div class="foot_echarts">
                <p style="margin: 0 0 0 20px; display: inline-block">同比</p>
                <svg
                  style="margin: -4px 0; display: inline-block"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M5.83334 11.6667L10 7.5L14.1667 11.6667H5.83334Z"
                    fill="#0FA465"
                  />
                </svg>
                <p style="display: inline-block; margin: 0">3</p>
                <p style="margin: 0 0 0 20px; display: inline-block">环比</p>
                <svg
                  style="margin: -4px 0; display: inline-block"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M5.83334 11.6667L10 7.5L14.1667 11.6667H5.83334Z"
                    fill="#EB1A09"
                  />
                </svg>
                <p style="display: inline-block; margin: 0">108</p>
              </div>
            </el-col>
            <el-col :span="6" class="echarts">
              <div class="title-left" />
              <div class="title">已办结转让类业务量</div>
              <div class="title_number">826</div>
              <div ref="business_transfer" class="echarts-style" />
              <div class="foot_echarts">
                <p style="margin: 0 0 0 20px; display: inline-block">同比</p>
                <svg
                  style="margin: -4px 0; display: inline-block"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M5.83334 11.6667L10 7.5L14.1667 11.6667H5.83334Z"
                    fill="#0FA465"
                  />
                </svg>
                <p style="display: inline-block; margin: 0">3</p>
                <p style="margin: 0 0 0 20px; display: inline-block">环比</p>
                <svg
                  style="margin: -4px 0; display: inline-block"
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M5.83334 11.6667L10 7.5L14.1667 11.6667H5.83334Z"
                    fill="#EB1A09"
                  />
                </svg>
                <p style="display: inline-block; margin: 0">108</p>
              </div>
            </el-col>
          </el-row>
        </div>
      </div>

      <div class="business-handling">
        <el-row>
          <el-col :span="24">
            <div ref="business_handle" class="business-style" />

            <!-- <Business /> -->
          </el-col>
        </el-row>
      </div>
    </div>
  </div>
</template>

<script>
import * as echarts from "echarts";
export default {
  components: {},
  data() {
    return {
      mainHeight: 0,
      value1: [new Date(2000, 10, 10, 10, 10), new Date(2000, 10, 11, 10, 10)],
      radio: 3,
      echartsData: [
        { name: "business_acting" },
        { name: "business_finish" },
        { name: "business_share" },
        { name: "business_transfer" },
        { name: "website_transferor" },
        { name: "website_assignee" },
        { name: "website_proxy" },
        { name: "website_user" },
        { name: "business_handle" },
      ],
      showsum: 200,
      showtransferorNumber: 50,
      transferorPercent: 0.25,
      showtransfereeNumber: 80,
      transfereePercent: 0.4,
      showagencyNumber: 100,
      agencyPercent: 0.5,
      showvisitorNumber: 150,
      visitorPercent: 0.75,
    };
  },
  created() {},
  mounted() {
    this.getEcharts();
  },
  methods: {
    // echarts渲染
    getEcharts() {
      let myChart;
      let option;

      this.echartsData.forEach((item) => {
        // if (this.$refs[item.name] === null) {
        //   return;
        // }
        // echarts.dispose(this.$refs[item.name]);
        myChart = echarts.init(this.$refs[item.name]);
        switch (item.name) {
          case "website_transferor":
            option = {
              grid: {
                left: "0",
                top: "60",
                width: 270,
                right: "0",
                bottom: "0",
              },
              xAxis: {
                type: "value",
                splitLine: { show: false },
                axisLabel: { show: false },
                axisTick: { show: false },
                axisLine: { show: false },
              },
              yAxis: {
                type: "category",
                axisTick: { show: false },
                axisLine: { show: false },
                axisLabel: { show: false },
              },

              series: [
                {
                  name: "",
                  type: "bar",
                  barWidth: 8,
                  data: [this.showtransferorNumber],
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                    color: "#0A6CF2",
                  },
                  zlevel: 1, // 柱状图所有图形的 zlevel 值,
                  // zlevel 大的 Canvas 会放在 zlevel 小的 Canvas 的上面
                },
                {
                  name: "",
                  type: "bar",
                  barGap: "-100%",
                  barWidth: 8,
                  data: [this.showsum],
                  color: "rgba(0,0,0,.07)",
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                  },
                },
              ],
            };
            break;
          case "website_assignee":
            option = {
              grid: {
                left: "0",
                top: "60",
                width: 270,
                right: "0",
                bottom: "0",
              },
              xAxis: {
                type: "value",
                splitLine: { show: false },
                axisLabel: { show: false },
                axisTick: { show: false },
                axisLine: { show: false },
              },
              yAxis: {
                type: "category",
                axisTick: { show: false },
                axisLine: { show: false },
                axisLabel: { show: false },
              },

              series: [
                {
                  name: "",
                  type: "bar",
                  barWidth: 8,
                  data: [this.showtransfereeNumber],
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                    color: "#F2900A",
                  },
                  zlevel: 1,
                },
                {
                  name: "",
                  type: "bar",
                  barGap: "-100%",
                  barWidth: 8,
                  data: [this.showsum],
                  color: "rgba(0,0,0,.07)",
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                  },
                },
              ],
            };
            break;
          case "website_proxy":
            option = {
              grid: {
                left: "0",
                top: "60",
                width: 270,
                right: "0",
                bottom: "0",
              },
              xAxis: {
                type: "value",
                splitLine: { show: false },
                axisLabel: { show: false },
                axisTick: { show: false },
                axisLine: { show: false },
              },
              yAxis: {
                type: "category",
                axisTick: { show: false },
                axisLine: { show: false },
                axisLabel: { show: false },
              },

              series: [
                {
                  name: "",
                  type: "bar",
                  barWidth: 8,
                  data: [this.showagencyNumber],
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                    color: "#0FA465",
                  },
                  zlevel: 1,
                },
                {
                  name: "",
                  type: "bar",
                  barGap: "-100%",
                  barWidth: 8,
                  data: [this.showsum],
                  color: "rgba(0,0,0,.07)",
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                  },
                },
              ],
            };
            break;
          case "website_user":
            option = {
              grid: {
                left: "0",
                top: "60",
                width: 270,
                right: "0",
                bottom: "0",
              },
              xAxis: {
                type: "value",
                splitLine: { show: false },
                axisLabel: { show: false },
                axisTick: { show: false },
                axisLine: { show: false },
              },
              yAxis: {
                type: "category",
                axisTick: { show: false },
                axisLine: { show: false },
                axisLabel: { show: false },
              },

              series: [
                {
                  name: "",
                  type: "bar",
                  barWidth: 8,
                  data: [this.showvisitorNumber],
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                    color: "#8794AE",
                  },
                  zlevel: 1,
                },
                {
                  name: "",
                  type: "bar",
                  barGap: "-100%",
                  barWidth: 8,
                  data: [this.showsum],
                  color: "rgba(0,0,0,.07)",
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                  },
                },
              ],
            };
            break;
          case "business_acting":
            option = {
              tooltip: {
                trigger: "axis",
                axisPointer: {
                  type: "none",
                },
                extraCssText: "width:180px;height:85px;background:#fff;",
                textStyle: {
                  fontSize: 14,
                },
                formatter: function () {
                  return (
                    "总业务量" +
                    "<br/>" +
                    ' <p style="color:#000; margin-top:10px;font-weight:bold;font-size: 24px;">' +
                    "423234" +
                    "</p>"
                  );
                },
              },
              grid: {
                left: "22",
                top: "10",
                width: 270,
                right: "0",
                bottom: "0",
              },
              xAxis: {
                type: "value",
                splitLine: { show: false },
                axisLabel: { show: false },
                axisTick: { show: false },
                axisLine: { show: false },
              },
              yAxis: {
                type: "category",
                axisTick: { show: false },
                axisLine: { show: false },
                axisLabel: { show: false },
              },

              series: [
                {
                  name: "",
                  type: "bar",
                  barWidth: 8,
                  data: [130],
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                    color: "#0A6CF2",
                  },
                  zlevel: 1,
                },
                {
                  name: "",
                  type: "bar",
                  barGap: "-100%",
                  barWidth: 8,
                  data: [200],
                  color: "rgba(0,0,0,.07)",
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                  },
                },
              ],
            };
            break;
          case "business_finish":
            option = {
              tooltip: {
                trigger: "axis",
                axisPointer: {
                  type: "none",
                },
                extraCssText: "width:180px;height:85px;background:#fff;",
                textStyle: {
                  fontSize: 14,
                },
                formatter: function () {
                  return (
                    "总业务量" +
                    "<br/>" +
                    ' <p style="color:#000; margin-top:10px;font-weight:bold;font-size: 24px;">' +
                    "423234" +
                    "</p>"
                  );
                },
              },
              grid: {
                left: "22",
                top: "10",
                width: 270,
                right: "0",
                bottom: "0",
              },
              xAxis: {
                type: "value",
                splitLine: { show: false },
                axisLabel: { show: false },
                axisTick: { show: false },
                axisLine: { show: false },
              },
              yAxis: {
                type: "category",
                axisTick: { show: false },
                axisLine: { show: false },
                axisLabel: { show: false },
              },

              series: [
                {
                  name: "",
                  type: "bar",
                  barWidth: 8,
                  data: [130],
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                    color: "#0A6CF2",
                  },
                  zlevel: 1,
                },
                {
                  name: "",
                  type: "bar",
                  barGap: "-100%",
                  barWidth: 8,
                  data: [200],
                  color: "rgba(0,0,0,.07)",
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                  },
                },
              ],
            };
            break;
          case "business_share":
            option = {
              tooltip: {
                trigger: "axis",
                axisPointer: {
                  type: "none",
                },
                extraCssText: "width:180px;height:85px;background:#fff;",
                textStyle: {
                  fontSize: 14,
                },
                formatter: function () {
                  return (
                    "总业务量" +
                    "<br/>" +
                    ' <p style="color:#000; margin-top:10px;font-weight:bold;font-size: 24px;">' +
                    "423234" +
                    "</p>"
                  );
                },
              },
              grid: {
                left: "22",
                top: "10",
                width: 270,
                right: "0",
                bottom: "0",
              },
              xAxis: {
                type: "value",
                splitLine: { show: false },
                axisLabel: { show: false },
                axisTick: { show: false },
                axisLine: { show: false },
              },
              yAxis: {
                type: "category",
                axisTick: { show: false },
                axisLine: { show: false },
                axisLabel: { show: false },
              },

              series: [
                {
                  name: "",
                  type: "bar",
                  barWidth: 8,
                  data: [130],
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                    color: "#0A6CF2",
                  },
                  zlevel: 1,
                },
                {
                  name: "",
                  type: "bar",
                  barGap: "-100%",
                  barWidth: 8,
                  data: [200],
                  color: "rgba(0,0,0,.07)",
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                  },
                },
              ],
            };
            break;
          case "business_transfer":
            option = {
              tooltip: {
                trigger: "axis",
                axisPointer: {
                  type: "none",
                },
                extraCssText: "width:180px;height:85px;background:#fff;",
                textStyle: {
                  fontSize: 14,
                },
                formatter: function () {
                  return (
                    "总业务量" +
                    "<br/>" +
                    ' <p style="color:#000; margin-top:10px;font-weight:bold;font-size: 24px;">' +
                    "423234" +
                    "</p>"
                  );
                },
              },
              grid: {
                // 直角坐标系内绘图网格
                left: "22",
                top: "10",
                width: 270,
                right: "0",
                bottom: "0",
              },
              xAxis: {
                type: "value",
                splitLine: { show: false }, // 坐标轴在 grid 区域中的分隔线
                axisLabel: { show: false }, // 坐标轴刻度标签
                axisTick: { show: false }, // 坐标轴刻度
                axisLine: { show: false }, // 坐标轴轴线
              },
              yAxis: {
                type: "category",
                axisTick: { show: false },
                axisLine: { show: false },
                axisLabel: { show: false }, // 坐标轴刻度标签
              },

              series: [
                {
                  name: "", // 系列名称
                  type: "bar", // 柱状、条形图
                  barWidth: 8, // 柱条的宽度,默认自适应
                  data: [130], // 系列中数据内容数组
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                    color: "#0A6CF2",
                  },
                  zlevel: 1, // 柱状图所有图形的 zlevel 值,
                  // zlevel 大的 Canvas 会放在 zlevel 小的 Canvas 的上面
                },
                {
                  name: "",
                  type: "bar",
                  barGap: "-100%",
                  barWidth: 8,
                  data: [200],
                  color: "rgba(0,0,0,.07)", // 柱条颜色
                  itemStyle: {
                    borderRadius: [0, 10, 10, 0],
                  },
                },
              ],
            };
            break;
          case "business_handle":
            option = {
              title: {
                text: "业务办理趋势图",
                x: "30px",
                y: "30px",
              },
              grid: {
                x: "5%", // x 偏移量
                y: "25%", // y 偏移量
                width: "90%", // 宽度
                height: "60%", // 高度
              },
              legend: {
                top: "30px",
                left: "85%",
                orient: "horizontal",
                itemWidth: 7,
                itemHeight: 7,
                align: "left",
                icon: "circle",
                data: ["代办业务", "已办业务"],
                textStyle: {
                  color: "#000", // 图例文字颜色
                  fontSize: 14,
                },
                itemGap: 30,
              },
              color: ["#0180ff", "#E1E4EB"], // 设置图例的颜色
              xAxis: {
                type: "category",
                data: [
                  "8.18",
                  "8.19",
                  "8.20",
                  "8.21",
                  "8.22",
                  "8.23",
                  "8.24",
                  "8.25",
                  "8.26",
                ],
                axisTick: { show: false },
                axisLine: { show: false },
              },
              yAxis: {
                type: "value",
                show: true,
                splitLine: { show: true },
                max: 60,
                minInterval: 20,
              },
              series: [
                {
                  name: "代办业务",
                  data: [2, 19, 10, 25, 45, 38, 55, 35, 23],
                  type: "line",
                  smooth: true,
                  // color: '#e4f2ff',
                  symbol: "none", // 取消折点圆圈
                  lineStyle: {
                    width: 3,
                    type: "solid",
                    color: "#0180ff", // 折线的颜色
                  },
                  areaStyle: {
                    color: {
                      x: 0,
                      y: 0,
                      x2: 0,
                      y2: 1,
                      colorStops: [
                        {
                          offset: 0,
                          color: "#81befd", // 0% 处的颜色
                        },
                        {
                          offset: 0.3,
                          color: "#e4f2ff", // 100% 处的颜色
                        },
                        {
                          offset: 1,
                          color: "#fff", // 100% 处的颜色
                        },
                      ],
                      globalCoord: false, // 缺省为 false
                    },
                  },
                },
                {
                  name: "已办业务",
                  data: [22, 15, 22, 42, 30, 11, 8, 22, 8],
                  type: "line",
                  smooth: true,
                  symbol: "none", // 取消折点圆圈
                  lineStyle: {
                    width: 2,
                    type: "solid",
                    color: "#E1E4EB", // 折线的颜色
                  },
                },
              ],
            };
            break;
        }
        myChart.setOption(option);
      });
    },
  },
};
</script>
<style lang="scss" scoped>
::v-deep {
  .content-box {
    padding: 0;
    background-color: #e7f1fb;
  }
  .el-radio__inner {
    width: 15px;
    height: 15px;
    border: 2px solid #dcdfe6;
  }
  .el-radio__inner:hover {
    width: 15px;
    height: 15px;
    border: 2px solid #f2900a;
  }
  .el-radio__input.is-checked .el-radio__inner {
    border-color: #f2900a;
    background: #fff;
  }
  .el-radio__input.is-checked + .el-radio__label,
  .el-radio {
    color: #000;
  }
  .el-radio__inner::after {
    background-color: #f2900a;
    width: 7.5px;
    height: 7.5px;
  }
}
.home {
  background-color: #e7f1fb;
  padding: 20px;
  min-height: calc(100vh - 150px);
}
.app-wrap {
  //min-height: calc(100vh - 115px - 20px);
  background-color: #e7f1fb;
  .wrap-div {
    width: 25%;
    height: 100%;
    float: left;
  }
  .business-warp {
    background-color: #fff;
    border-radius: 8px;
    height: 229px;
    margin: 0 0 20px 0;
    .top {
      padding-top: 15px;
      //background-color: #444444;
      .block {
        display: inline;
      }
      .radio {
        display: inline;
        margin-left: 30px;
      }
      .demonstration {
        font-size: 14px;
        line-height: 20px;
        text-align: right;
        margin: 27px 8px 27px 20px;
      }
    }
    .bottom {
      background-color: #fff;
      padding: 0 20px;
    }
  }
  .website-warp {
    background-color: #fff;
    border-radius: 8px;
    height: 158px;
    margin: 0 0 20px 0;
    .website {
      padding: 10px 20px;
      //border: 1px solid red;
    }
    .website-style {
      height: 110px;
      //border: 1px solid blue;
    }
  }
  .business-handling {
    background-color: #fff;
    border-radius: 8px;
    height: 337px;
    margin: 0 0 20px 0;
  }
  .business-style {
    margin: 0px 20px;
    height: 337px;
    //border: 1px solid blue;
  }
}

.echarts {
  padding: 10px 0px;
  //border: 1px solid red;
}
.echarts-style {
  width: 100%;
  height: 50px;
  //border: 1px solid blue;
}
.title {
  font-weight: 500;
  font-size: 16px;
  color: #001d3b;
  margin-left: 5px;
  line-height: 23px;
  float: left;
}
.title-left {
  height: 15px;
  width: 2px;
  background: #0a6cf2;
  border-radius: 100px;
  margin-left: 20px;
  margin-top: 4px;
  float: left;
}
.title_number {
  margin: 30px 0 10px 25px;
  font-weight: bold;
  font-size: 22px;
  line-height: 28px;
  color: #001d3b;
}
.logo,
.left {
  margin-top: 10px;
  float: left;
  margin-right: 10px;
}
.title-top {
  font-size: 14px;
  line-height: 20px;
  color: #8794ae;
}
.title-num {
  font-weight: bold;
  font-size: 22px;
  line-height: 28px;
  color: #001d3b;
}
.foot {
  font-size: 14px;
  line-height: 20px;
  color: #000000;
}
</style>
