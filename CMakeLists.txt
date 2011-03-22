project(SLSmackdown NONE)

cmake_minimum_required(VERSION 2.8)

include(UseLATEX.cmake)

set(images
  images/TransparentOutput.png
  images/OpaqueOutput.png
  )

add_latex_document(SLSmackdown.tex
  BIBFILES SLSmackdown.bib
  IMAGES ${images}
  )
