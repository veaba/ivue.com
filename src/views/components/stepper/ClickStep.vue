<template>
      <IvueStepper :current-step="current">
            <IvueStepperStep title="已完成" content="这里是该步骤的描述信息" editable></IvueStepperStep>
            <IvueStepperStep title="进行中" content="这里是该步骤的描述信息" editable></IvueStepperStep>
            <IvueStepperStep title="待进行" content="这里是该步骤的描述信息" editable></IvueStepperStep>
            <IvueStepperStep title="待进行" content="这里是该步骤的描述信息" editable></IvueStepperStep>
      </IvueStepper>
</template>

<script>
export default {
      data () {
            return {
                  current: 1
            }
      }
}
</script>
