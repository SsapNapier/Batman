<template lang="jade">
div.sidebar
  a.active.main Войти&nbsp;&nbsp;&nbsp;&#8594;
  div.bar
    a {{ greeting }}
    hr
    a Ж/Д Авиабилеты
    hr
    a Гостиницы
    hr
    a Страхование
    hr
    a Трансфер
</template>

<script>
    module.exports = {
        data: function() {
            return {
                greeting: 'Авиабилеты'
            }
        }
    }
</script>

<style lang="sass?indentedSyntax=true">
.sidebar
  font-family: SegoeUI
  font-size: 12px
  flex-basis: 254px
  border-left: 1px solid #c5c5c5
  height: 966px
  align-items: flex-end

hr
  position: relative
  top: 89px
  left: 45px
  margin-left: 0
  width: 5%
  margin-bottom: 15%


.bar
  position: relative
  top: 171px

a
  position: relative
  top: 92px
  left: 45px
  color: #c5c5c5
  display: flex
  flex-direction: column
  padding-bottom: 14%

  &.active
    color: #00aeef
    padding-bottom: 14px
    text-decoration: none
    cursor: pointer

</style>
