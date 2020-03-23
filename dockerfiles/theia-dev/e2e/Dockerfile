# Copyright (c) 2018-2019 Red Hat, Inc.
# This program and the accompanying materials are made
# available under the terms of the Eclipse Public License 2.0
# which is available at https://www.eclipse.org/legal/epl-2.0/
#
# SPDX-License-Identifier: EPL-2.0

# Use upstream image
FROM ${BUILD_ORGANIZATION}/${BUILD_PREFIX}-theia-dev:${BUILD_TAG}

# Just try to build the latest theia with current image
RUN git clone -b 'master' --single-branch --depth 1 https://github.com/eclipse-theia/theia theia

# setup extra step
#{INCLUDE:docker/${BUILD_IMAGE_TARGET}/post-clone.dockerfile}

RUN cd theia && yarn
