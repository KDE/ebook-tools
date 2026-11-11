# SPDX-FileCopyrightText: 2007 Ely Levy <elylevy@cs.huji.ac.il>
#
# SPDX-License-Identifier: MIT

add_subdirectory (libepub)
if(BUILD_TOOLS)
  add_subdirectory (tools)
endif()

