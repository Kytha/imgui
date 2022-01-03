SET ( GLAD_SOURCE
      imgui_demo.cpp
      imgui_draw.cpp
      imgui_tables.cpp
      imgui_widgets.cpp
      imgui.cpp
  )

SET ( GLAD_HEADERS
    imgui.h
    imgui_internal.h
    imconfig.h
    imstb_rectpack.h
    imstb_textedit.h
    imstb_truetype.h
  )

ADD_LIBRARY ( Glad STATIC
  ${GLAD_SOURCE}
  ${GLAD_HEADERS}
  )

TARGET_INCLUDE_DIRECTORIES(Glad PUBLIC /backends)
