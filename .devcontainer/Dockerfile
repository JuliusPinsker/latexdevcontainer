FROM qmcgaw/latexdevcontainer:latest-full

# Install required fonts for dissertation
RUN apt-get update && apt-get install -y \
    fonts-ebgaramond \
    fonts-lato \
    fonts-noto \
    fonts-noto-mono \
    fonts-liberation \
    fontconfig \
    && fc-cache -fv \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Update font cache to ensure all fonts are available
RUN fc-cache -fv

# Set default shell to zsh
SHELL ["/bin/zsh", "-c"]
