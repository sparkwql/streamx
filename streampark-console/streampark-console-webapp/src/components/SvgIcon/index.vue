<!--

    Licensed to the Apache Software Foundation (ASF) under one or more
    contributor license agreements.  See the NOTICE file distributed with
    this work for additional information regarding copyright ownership.
    The ASF licenses this file to You under the Apache License, Version 2.0
    (the "License"); you may not use this file except in compliance with
    the License.  You may obtain a copy of the License at

       https://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

-->

<template>
  <span :class="'svg-icon-'.concat(size).concat(border? ' svg-icon-border':'')" class="anticon">
    <alarm v-if="name==='alarm'"></alarm>
    <testalarm v-if="name==='testalarm'"></testalarm>
    <analyse v-if="name==='analyse'"></analyse>
    <flink v-if="name==='flink'"></flink>
    <spark v-if="name==='spark'"></spark>
    <fql v-if="name==='fql'"></fql>
    <flinksql v-if="name==='flinksql'"></flinksql>
    <maven v-if="name==='maven'"></maven>
    <mvnpass v-if="name==='mvnpass'"></mvnpass>
    <workspace v-if="name==='workspace'"></workspace>
    <threshold v-if="name==='threshold'"></threshold>
    <http v-if="name==='http'"></http>
    <deploy v-if="name==='deploy'"></deploy>
    <stream v-if="name==='stream'"></stream>
    <format v-if="name==='format'"></format>
    <dingtalk v-if="name==='dingtalk'"></dingtalk>
    <lark v-if="name==='lark'"></lark>
    <mail v-if="name==='mail'"></mail>
    <sms v-if="name==='sms'"></sms>
    <message v-if="name==='message'"></message>
    <wechat v-if="name==='wechat'"></wechat>
    <wecom v-if="name==='wecom'"></wecom>
    <host v-if="name==='host'"></host>
    <keys v-if="name==='keys'"></keys>
    <port v-if="name==='port'"></port>
    <ssl v-if="name==='ssl'"></ssl>
    <theme v-if="name==='theme'"></theme>
    <question v-if="name==='question'"></question>
    <remove v-if="name==='remove'"></remove>
    <edit v-if="name==='edit'"></edit>
    <mapping v-if="name==='mapping'"></mapping>
    <pause v-if="name==='pause'"></pause>
    <play v-if="name==='play'"></play>
    <see v-if="name==='see'"></see>
    <shutdown v-if="name==='shutdown'"></shutdown>
    <thunderbolt v-if="name==='thunderbolt'"></thunderbolt>
    <rollback v-if="name==='rollback'"></rollback>
    <upload v-if="name==='upload'"></upload>
    <plus v-if="name==='plus'"></plus>
    <flame v-if="name==='flame'"></flame>
    <icode v-if="name==='code'"></icode>
    <copy v-if="name==='copy'"></copy>
    <swap v-if="name==='swap'"></swap>
    <github v-if="name==='github'"></github>
    <resetpass v-if="name==='resetpass'"></resetpass>
    <sun v-if="name==='sun'"></sun>
    <moon v-if="name==='moon'"></moon>
    <user v-if="name==='user'"></user>
    <docker v-if="name==='docker'"></docker>
    <namespace v-if="name==='namespace'"></namespace>
    <auth v-if="name==='auth'"></auth>
    <password v-if="name==='password'"></password>
  </span>
</template>

<script>
import {
  alarm,
  testalarm,
  analyse,
  deploy,
  flink,
  flinksql,
  fql,
  http,
  maven,
  mvnpass,
  spark,
  stream,
  workspace,
  threshold,
  format,
  dingtalk,
  lark,
  mail,
  sms,
  message,
  wechat,
  wecom,
  host,
  keys,
  port,
  ssl,
  theme,
  question,
  remove,
  edit,
  mapping,
  pause,
  play,
  see,
  shutdown,
  thunderbolt,
  rollback,
  upload,
  plus,
  flame,
  icode,
  copy,
  swap,
  github,
  resetpass,
  sun,
  moon,
  user,
  docker,
  namespace,
  auth,
  password
} from '@/core/icons'

export default {
  name: 'SvgIcon',
  components: {
    alarm,
    testalarm,
    analyse,
    deploy,
    flink,
    flinksql,
    fql,
    http,
    maven,
    mvnpass,
    spark,
    stream,
    workspace,
    threshold,
    format,
    dingtalk,
    lark,
    mail,
    sms,
    message,
    wechat,
    wecom,
    host,
    keys,
    port,
    ssl,
    theme,
    question,
    remove,
    edit,
    mapping,
    pause,
    play,
    see,
    shutdown,
    thunderbolt,
    rollback,
    upload,
    plus,
    flame,
    icode,
    copy,
    swap,
    github,
    resetpass,
    sun,
    moon,
    user,
    docker,
    namespace,
    auth,
    password
  },
  props: {
    name: {
      type: String,
      default: ''
    },
    size: {
      type: String,
      default: 'default'
    },
    border: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style scoped lang="less">

.svg-icon-default > svg {
  height: 1.05em !important;
  max-width: 1.05em !important;
  cursor: pointer;
}

.svg-icon-border {
  background: @border-color-split;
  border-radius: 50% ;
  margin-left: 2px;
}

.svg-icon-min > svg {
  max-height: 15px !important;
  max-width: 15px !important;
}

.svg-icon-small > svg {
  max-height: 20px !important;
  max-width: 20px !important;
}

.svg-icon-middle > svg {
  max-height: 25px !important;
  max-width: 25px !important;
}

.svg-icon-large > svg {
  max-height: 50px !important;
  max-width: 50px !important;
}
</style>
