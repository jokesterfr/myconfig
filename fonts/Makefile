# -----------------------------------------------------------------------------
# @author Clément Désiles <main@jokester.fr>
# @date   2015-02-05
# -----------------------------------------------------------------------------
NAME        = fonts
FONTS_DIR   = $(HOME)/.local/share/fonts
LOCAL_DIR   = $(shell pwd)

all: check install

install: source_code_pro
	fc-cache -f $(FONTS_DIR)

source_code_pro: $(FONTS_DIR)/Sauce\ Code\ Powerline\ Regular.otf

$(FONTS_DIR): ; mkdir -p $(FONTS_DIR)
$(FONTS_DIR)/Sauce\ Code\ Powerline\ Regular.otf: $(FONTS_DIR); cp SourceCodePro/*.otf $(FONTS_DIR)

check: git-installed
git-installed: ; @which git > /dev/null
fc-cache-installed: ; @which fc-cache > /dev/null
