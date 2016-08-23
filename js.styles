$(document).ready ->
  
  items = [
    ".ease",
    ".ease-in",
    ".ease-out",
    ".ease-in-out",
    ".cubic-bezier"
  ]
  
  resetColor = () ->
    $(".ease").css("color": "rgba(255,255,255, .2)")
    $(".ease-in").css("color": "rgba(255,255,255, .2)")
    $(".ease-out").css("color": "rgba(255,255,255, .2)")
    $(".ease-in-out").css("color": "rgba(255,255,255, .2)")
    $(".cubic-bezier").css("color": "rgba(255,255,255, .2)")
    
  
  clickOnItem = (itemName) ->
    $(itemName).on "click", ->
      resetColor()
      $(@).css("color": "rgba(255,255,255, .8)")
      switch itemName
        when ".ease"
          setTimeFunction("ease")
        when ".ease-in"
          setTimeFunction("ease-in")
        when ".ease-out"
          setTimeFunction("ease-out")
        when ".ease-in-out"
          setTimeFunction("ease-in-out")
        when ".cubic-bezier"
          setTimeFunction("cubic-bezier(0,.8,1,.2)")
    
  setTimeFunction = (timeFunction) ->
    $(".dot").css("animation-timing-function": timeFunction)
  
  for item in items
    clickOnItem(item)
    console.log item
