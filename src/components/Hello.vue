<template>
  <div>
    <span class='tittle'>
      欢迎登陆
    </span>
    <divider>Vue Vux</divider>
    <Group>
      <XInput tittle='账号' v-model='account' placeholder='账号' type=text>
        
      </XInput>
    </Group>
    <x-input tittle='密码' v-model='password' placeholder='密码' type='password'></x-input>
    <XButton type="primary" action-type="button">登陆</XButton>
    
  </div>
</template>

<script>
import { Divider, Group, XInput, XButton } from 'vux'
export default {
  components: {
    Divider,
    Group,
    XInput,
    XButton
  },
  data () {
    return {
      account: '',
      password: ''
    }
  }
}
</script>
