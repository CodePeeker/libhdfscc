SET(SRC_DIR ${CONTRIB_SOURCE_DIR}/protobuf)

# EXECUTE_PROCESS(
#     WORKING_DIRECTORY ${SRC_DIR}
#     COMMAND_ECHO STDOUT
#     COMMAND mkdir -p ${SRC_DIR}/build
#     COMMAND cmake -DCMAKE_CXX_STANDARD=17 -DCMAKE_INSTALL_PREFIX=${WORKSPACE_INSTALL_DIR} -Dprotobuf_ABSL_PROVIDER=package -DCMAKE_PREFIX_PATH=${WORKSPACE_INSTALL_DIR} -S ${SRC_DIR} -B ${SRC_DIR}/build
#     COMMAND cmake --build ${SRC_DIR}/build --target install
# )

FIND_PACKAGE(Protobuf REQUIRED GLOBAL)
