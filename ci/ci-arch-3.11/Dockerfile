ARG PACMAN_INSTALL_COMMAND="pacman -S --noconfirm"

FROM archlinux:latest
ARG PACMAN_INSTALL_COMMAND

RUN pacman -Syu --noconfirm \
    && pacman -Sc --noconfirm

RUN ${PACMAN_INSTALL_COMMAND} \
    base-devel cmake git curl \
    boost fftw \
    python python-numpy python-mako python-packaging python-yaml \
    pybind11 \
    spdlog \
    gsl \
    libvolk \
    gmp \
    qt6-base qt6-tools qt6-svg \
    qwt \
    python-pyqt6 \
    zeromq cppzmq \
    python-gobject \
    python-cairo \
    gtk3 \
    python-jsonschema \
    && pacman -Sc --noconfirm
RUN ${PACMAN_INSTALL_COMMAND} \
    libiio \
    libuhd \
    soapysdr \
    python-click \
    sdl_image \
    python-pytest \
    python-pytest-qt \
    libsndfile \
    python-pyqtgraph \
    python-colorama \
    python-scipy \
    python-pygccxml \
    && pacman -Sc --noconfirm

