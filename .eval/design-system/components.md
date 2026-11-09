# Components

Every row is an applied `// @uxid` identifier. Ids are path-derived and permanent.

| identifier | file | flow | type | description |
| --- | --- | --- | --- | --- |
| `apps/browser-extension/src/BookmarkDeletedPage::BookmarkDeletedPage` | apps/browser-extension/src/BookmarkDeletedPage.tsx | all | component | Function component. Renders: div, p, Trash2. |
| `apps/browser-extension/src/BookmarkSavedPage::BookmarkSavedPage` | apps/browser-extension/src/BookmarkSavedPage.tsx | all | component | Function component. Hooks: useParams, useNavigate, useState, useDeleteBookmark, usePluginSettings, useAutoRefreshingBookmarkQuery. Renders: div, p, a, ErrorCallout, CircleCheck, ExternalLink, Button, Spinner, +1 more. |
| `apps/browser-extension/src/BookmarkSavedPage::Section` | apps/browser-extension/src/BookmarkSavedPage.tsx | all | component | Function component. Props: title, children. Renders: section, h3. |
| `apps/browser-extension/src/components/BookmarkLists::BookmarkLists` | apps/browser-extension/src/components/BookmarkLists.tsx | all | component | Function component. Props: bookmarkId. Hooks: useTRPC, useBookmarkLists, useRemoveBookmarkFromList, useQuery. Renders: div, button, ListPathLabel, X. |
| `apps/browser-extension/src/components/BookmarkLists::ListPathLabel` | apps/browser-extension/src/components/BookmarkLists.tsx | all | component | Function component. Props: path. Renders: span. |
| `apps/browser-extension/src/components/ErrorCallout::ErrorCallout` | apps/browser-extension/src/components/ErrorCallout.tsx | all | component | Function component. Props: title, children, className. Renders: div, p, CircleAlert. |
| `apps/browser-extension/src/components/ListsSelector::ListsSelector` | apps/browser-extension/src/components/ListsSelector.tsx | all | component | Function component. Props: bookmarkId. Hooks: useTRPC, useSet, useState, useAddBookmarkToList, useRemoveBookmarkFromList, useQuery, +1 more. Renders: Popover, PopoverTrigger, Button, Plus, DynamicPopoverContent, Command. |
| `apps/browser-extension/src/components/NoteEditor::NoteEditor` | apps/browser-extension/src/components/NoteEditor.tsx | all | component | Function component. Props: bookmarkId. Hooks: useAutoRefreshingBookmarkQuery, useState, useEffect, useUpdateBookmark. Renders: div, p, Textarea, Check, Button, Spinner. |
| `apps/browser-extension/src/components/PopupHeader::HeaderIconButton` | apps/browser-extension/src/components/PopupHeader.tsx | all | component | Function component. Props: label, ...props. Renders: Button. |
| `apps/browser-extension/src/components/PopupHeader::PopupHeader` | apps/browser-extension/src/components/PopupHeader.tsx | all | component | Function component. Props: title, onBack, children. Renders: div, h1, Button, ArrowLeft, Logo. |
| `apps/browser-extension/src/components/StatusMessage::StatusMessage` | apps/browser-extension/src/components/StatusMessage.tsx | all | component | Function component. Props: label, detail. Renders: div, p, Spinner. |
| `apps/browser-extension/src/components/TagList::TagList` | apps/browser-extension/src/components/TagList.tsx | all | component | Function component. Props: bookmarkId. Hooks: useAutoRefreshingBookmarkQuery. Renders: Badge, Sparkles, Spinner. |
| `apps/browser-extension/src/components/TagsSelector::TagsSelector` | apps/browser-extension/src/components/TagsSelector.tsx | all | component | Function component. Props: bookmarkId. Hooks: useTRPC, useQuery, useAutoRefreshingBookmarkQuery, useState, useSet, useUpdateBookmarkTags. Renders: Popover, PopoverTrigger, Button, Plus, DynamicPopoverContent, Command. |
| `apps/browser-extension/src/components/TitleEditor::TitleEditor` | apps/browser-extension/src/components/TitleEditor.tsx | all | component | Function component. Props: bookmarkId. Hooks: useTRPC, useQueryClient, useAutoRefreshingBookmarkQuery, useState, useUpdateBookmark. Renders: div, p, span, Input, Button, Spinner, Check. |
| `apps/browser-extension/src/components/ui/badge::Badge` | apps/browser-extension/src/components/ui/badge.tsx | all | component | Function component. Props: className, variant, ...props. Renders: div. |
| `apps/browser-extension/src/components/ui/button::Button` | apps/browser-extension/src/components/ui/button.tsx | all | component | Wrapped component. Props: className, variant, size, asChild, ...props. Renders: Comp. |
| `apps/browser-extension/src/components/ui/command::Command` | apps/browser-extension/src/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: CommandPrimitive. |
| `apps/browser-extension/src/components/ui/command::CommandDialog` | apps/browser-extension/src/components/ui/command.tsx | all | component | Arrow function component. Props: children, ...props. Renders: Dialog, DialogContent, Command. |
| `apps/browser-extension/src/components/ui/command::CommandEmpty` | apps/browser-extension/src/components/ui/command.tsx | all | component | Wrapped component. Renders: CommandPrimitive.Empty. |
| `apps/browser-extension/src/components/ui/command::CommandGroup` | apps/browser-extension/src/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: CommandPrimitive.Group. |
| `apps/browser-extension/src/components/ui/command::CommandInput` | apps/browser-extension/src/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: div, Search, CommandPrimitive.Input. |
| `apps/browser-extension/src/components/ui/command::CommandItem` | apps/browser-extension/src/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: CommandPrimitive.Item. |
| `apps/browser-extension/src/components/ui/command::CommandList` | apps/browser-extension/src/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: CommandPrimitive.List. |
| `apps/browser-extension/src/components/ui/command::CommandSeparator` | apps/browser-extension/src/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: CommandPrimitive.Separator. |
| `apps/browser-extension/src/components/ui/command::CommandShortcut` | apps/browser-extension/src/components/ui/command.tsx | all | component | Arrow function component. Props: className, ...props. Renders: span. |
| `apps/browser-extension/src/components/ui/dialog::DialogContent` | apps/browser-extension/src/components/ui/dialog.tsx | all | component | Wrapped component. Props: className, children, ...props. Renders: span, DialogPortal, DialogOverlay, DialogPrimitive.Content, DialogPrimitive.Close, X. |
| `apps/browser-extension/src/components/ui/dialog::DialogDescription` | apps/browser-extension/src/components/ui/dialog.tsx | all | component | Wrapped component. Props: className, ...props. Renders: DialogPrimitive.Description. |
| `apps/browser-extension/src/components/ui/dialog::DialogFooter` | apps/browser-extension/src/components/ui/dialog.tsx | all | component | Arrow function component. Props: className, ...props. Renders: div. |
| `apps/browser-extension/src/components/ui/dialog::DialogHeader` | apps/browser-extension/src/components/ui/dialog.tsx | all | component | Arrow function component. Props: className, ...props. Renders: div. |
| `apps/browser-extension/src/components/ui/dialog::DialogOverlay` | apps/browser-extension/src/components/ui/dialog.tsx | all | component | Wrapped component. Props: className, ...props. Renders: DialogPrimitive.Overlay. |
| `apps/browser-extension/src/components/ui/dialog::DialogTitle` | apps/browser-extension/src/components/ui/dialog.tsx | all | component | Wrapped component. Props: className, ...props. Renders: DialogPrimitive.Title. |
| `apps/browser-extension/src/components/ui/dynamic-popover::DynamicPopoverContent` | apps/browser-extension/src/components/ui/dynamic-popover.tsx | all | component | Wrapped component. Props: className, align, sideOffset, dynamicHeight, debounceMs, children, +1 more. Hooks: useRef, useState, useDebounce, useEffect, useCallback, useLayoutEffect, +1 more. Renders: PopoverPrimitive.Portal, PopoverPrimitive.Content. |
| `apps/browser-extension/src/components/ui/input::Input` | apps/browser-extension/src/components/ui/input.tsx | all | component | Wrapped component. Props: className, type, ...props. Renders: input. |
| `apps/browser-extension/src/components/ui/popover::PopoverContent` | apps/browser-extension/src/components/ui/popover.tsx | all | component | Wrapped component. Props: className, align, sideOffset, ...props. Renders: PopoverPrimitive.Portal, PopoverPrimitive.Content. |
| `apps/browser-extension/src/components/ui/select::SelectContent` | apps/browser-extension/src/components/ui/select.tsx | all | component | Wrapped component. Props: className, children, position, ...props. Renders: SelectPrimitive.Portal, SelectPrimitive.Content, SelectScrollUpButton, SelectPrimitive.Viewport, SelectScrollDownButton. |
| `apps/browser-extension/src/components/ui/select::SelectItem` | apps/browser-extension/src/components/ui/select.tsx | all | component | Wrapped component. Props: className, children, ...props. Renders: span, SelectPrimitive.Item, SelectPrimitive.ItemIndicator, Check, SelectPrimitive.ItemText. |
| `apps/browser-extension/src/components/ui/select::SelectLabel` | apps/browser-extension/src/components/ui/select.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SelectPrimitive.Label. |
| `apps/browser-extension/src/components/ui/select::SelectScrollDownButton` | apps/browser-extension/src/components/ui/select.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SelectPrimitive.ScrollDownButton, ChevronDown. |
| `apps/browser-extension/src/components/ui/select::SelectScrollUpButton` | apps/browser-extension/src/components/ui/select.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SelectPrimitive.ScrollUpButton, ChevronUp. |
| `apps/browser-extension/src/components/ui/select::SelectSeparator` | apps/browser-extension/src/components/ui/select.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SelectPrimitive.Separator. |
| `apps/browser-extension/src/components/ui/select::SelectTrigger` | apps/browser-extension/src/components/ui/select.tsx | all | component | Wrapped component. Props: className, children, ...props. Renders: SelectPrimitive.Trigger, SelectPrimitive.Icon, ChevronDown. |
| `apps/browser-extension/src/components/ui/switch::Switch` | apps/browser-extension/src/components/ui/switch.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SwitchPrimitives.Root, SwitchPrimitives.Thumb. |
| `apps/browser-extension/src/components/ui/textarea::Textarea` | apps/browser-extension/src/components/ui/textarea.tsx | all | component | Wrapped component. Props: className, ...props. Renders: textarea. |
| `apps/browser-extension/src/Layout::Layout` | apps/browser-extension/src/Layout.tsx | all | component | Function component. Hooks: useNavigate, usePluginSettings. Renders: div, a, Spinner, Navigate, PopupHeader, House, HeaderIconButton, RefreshCw. |
| `apps/browser-extension/src/Logo::Logo` | apps/browser-extension/src/Logo.tsx | all | component | Function component. Props: className. Renders: span, img. |
| `apps/browser-extension/src/main::App` | apps/browser-extension/src/main.tsx | all | component | Function component. Renders: div, Providers, HashRouter, Routes, Route, Layout, SavePage. |
| `apps/browser-extension/src/OptionsPage::OptionsPage` | apps/browser-extension/src/OptionsPage.tsx | all | component | Function component. Hooks: useTRPC, useQueryClient, useNavigate, useLocation, usePluginSettings, useTheme, +4 more. Renders: span, div, Spinner, PopupHeader, SettingsSection, Button, LogOut, SettingsRow. |
| `apps/browser-extension/src/OptionsPage::SettingsRow` | apps/browser-extension/src/OptionsPage.tsx | all | component | Function component. Props: label, description, inset, children. Renders: div, span. |
| `apps/browser-extension/src/OptionsPage::SettingsSection` | apps/browser-extension/src/OptionsPage.tsx | all | component | Function component. Props: title, children. Renders: section, h2, div. |
| `apps/browser-extension/src/SavePage::SavePage` | apps/browser-extension/src/SavePage.tsx | all | component | Function component. Hooks: useTRPC, usePluginSettings, useState, useMutation, useEffect. Renders: form, h2, div, label, p, span, ErrorCallout, StatusMessage, +4 more. |
| `apps/browser-extension/src/ServerAddressPage::ServerAddressPage` | apps/browser-extension/src/ServerAddressPage.tsx | all | component | Function component. Hooks: useNavigate, usePluginSettings, useState, useEffect. Renders: div, section, label, p, h2, span, PopupHeader, ErrorCallout, +4 more. |
| `apps/browser-extension/src/SignInPage::SignInPage` | apps/browser-extension/src/SignInPage.tsx | all | component | Function component. Hooks: useTRPC, useNavigate, usePluginSettings, useState, useMutation. Renders: div, form, label, button, span, a, Logo, Input, +4 more. |
| `apps/browser-extension/src/Spinner::Spinner` | apps/browser-extension/src/Spinner.tsx | all | component | Function component. Props: className. Renders: svg, path. |
| `apps/browser-extension/src/utils/providers::Providers` | apps/browser-extension/src/utils/providers.tsx | all | component | Function component. Props: children. Hooks: usePluginSettings. Renders: TRPCSettingsProvider, ThemeProvider. |
| `apps/browser-extension/src/utils/ThemeProvider::ThemeProvider` | apps/browser-extension/src/utils/ThemeProvider.tsx | all | component | Function component. Props: children, ...props. Hooks: usePluginSettings, useEffect. Renders: ThemeProviderContext.Provider. |
| `apps/landing/components/ui/button::Button` | apps/landing/components/ui/button.tsx | all | component | Wrapped component. Props: className, variant, size, asChild, ...props. Renders: Comp. |
| `apps/landing/src/Apps::Apps` | apps/landing/src/Apps.tsx | all | component | Function component. Renders: div, main, h1, p, ListingSection. |
| `apps/landing/src/Apps::ListingSection` | apps/landing/src/Apps.tsx | all | component | Function component. Props: title, description, items. Renders: section, h2, p, div, a, img. |
| `apps/landing/src/components/ClosingCta::ClosingCta` | apps/landing/src/components/ClosingCta.tsx | all | component | Function component. Renders: section, div, h2, span, p, a. |
| `apps/landing/src/components/FeatureShowcase::FeatureShowcase` | apps/landing/src/components/FeatureShowcase.tsx | all | component | Function component. Props: label, headline, description, bullets, tint, reverse, +1 more. Renders: div, span, h3, p, ul, li. |
| `apps/landing/src/components/FeatureShowcase::FeatureShowcaseHalf` | apps/landing/src/components/FeatureShowcase.tsx | all | component | Function component. Props: label, headline, description, tint, children. Renders: div, span, h3, p. |
| `apps/landing/src/components/Footer::Footer` | apps/landing/src/components/Footer.tsx | all | component | Function component. Renders: footer, div, img, p, h3, ul. |
| `apps/landing/src/components/LlmReady::LlmReady` | apps/landing/src/components/LlmReady.tsx | all | component | Function component. Renders: section, div, span, h3, p, feature.icon, TerminalCard. |
| `apps/landing/src/components/OpenSource::OpenSource` | apps/landing/src/components/OpenSource.tsx | all | component | Function component. Renders: section, div, h2, p, a, Github, TerminalCard. |
| `apps/landing/src/components/Platforms::Platforms` | apps/landing/src/components/Platforms.tsx | all | component | Function component. Renders: section, div, p, a, img, ArrowUpRight. |
| `apps/landing/src/components/showcase/CollabListCardMockup::CollabListCardMockup` | apps/landing/src/components/showcase/CollabListCardMockup.tsx | all | component | Function component. Renders: div, span, MockupCard, Plus. |
| `apps/landing/src/components/showcase/MockupCard::MockupCard` | apps/landing/src/components/showcase/MockupCard.tsx | all | component | Function component. Props: className, children. Renders: div. |
| `apps/landing/src/components/showcase/MockupCard::TrafficDots` | apps/landing/src/components/showcase/MockupCard.tsx | all | component | Function component. Props: className. Renders: div. |
| `apps/landing/src/components/showcase/RssFeedsCardMockup::RssFeedsCardMockup` | apps/landing/src/components/showcase/RssFeedsCardMockup.tsx | all | component | Function component. Renders: div, span, MockupCard, Plus, Rss, Toggle. |
| `apps/landing/src/components/showcase/RssFeedsCardMockup::Toggle` | apps/landing/src/components/showcase/RssFeedsCardMockup.tsx | all | component | Function component. Renders: div. |
| `apps/landing/src/components/showcase/RuleCardMockup::RuleCardMockup` | apps/landing/src/components/showcase/RuleCardMockup.tsx | all | component | Function component. Renders: div, span, MockupCard, Workflow, StepLabel, StepRow, StepConnector, Plus. |
| `apps/landing/src/components/showcase/RuleCardMockup::StepConnector` | apps/landing/src/components/showcase/RuleCardMockup.tsx | all | component | Function component. Renders: div. |
| `apps/landing/src/components/showcase/RuleCardMockup::StepLabel` | apps/landing/src/components/showcase/RuleCardMockup.tsx | all | component | Function component. Props: children. Renders: span. |
| `apps/landing/src/components/showcase/RuleCardMockup::StepRow` | apps/landing/src/components/showcase/RuleCardMockup.tsx | all | component | Function component. Props: icon, children. Renders: div, Icon. |
| `apps/landing/src/components/showcase/ScreenshotCard::BrowserScreenshotCard` | apps/landing/src/components/showcase/ScreenshotCard.tsx | all | component | Function component. Props: src, alt, width, height. Renders: div, img, TrafficDots. |
| `apps/landing/src/components/showcase/ScreenshotCard::PaperScreenshotCard` | apps/landing/src/components/showcase/ScreenshotCard.tsx | all | component | Function component. Props: src, alt, width, height. Renders: div, img. |
| `apps/landing/src/components/showcase/SearchCardMockup::SearchCardMockup` | apps/landing/src/components/showcase/SearchCardMockup.tsx | all | component | Function component. Renders: div, span, result.tileIcon, MockupCard, Search, Sparkles, ChevronDown. |
| `apps/landing/src/components/showcase/TagsCardMockup::TagChip` | apps/landing/src/components/showcase/TagsCardMockup.tsx | all | component | Function component. Props: label, ai. Renders: span, Sparkles, X. |
| `apps/landing/src/components/showcase/TagsCardMockup::TagsCardMockup` | apps/landing/src/components/showcase/TagsCardMockup.tsx | all | component | Function component. Renders: span, div, MockupCard, Calendar, TagChip. |
| `apps/landing/src/components/TerminalCard::TerminalCard` | apps/landing/src/components/TerminalCard.tsx | all | component | Function component. Props: lines, className. Renders: div, span. |
| `apps/landing/src/components/UseCases::SearchModesIcon` | apps/landing/src/components/UseCases.tsx | all | component | Function component. Props: className. Renders: svg, path, circle. |
| `apps/landing/src/components/UseCases::UseCases` | apps/landing/src/components/UseCases.tsx | all | component | Function component. Renders: section, div, span, h2, p, FeatureShowcase, BrowserScreenshotCard, SearchCardMockup, +3 more. |
| `apps/landing/src/Homepage::Homepage` | apps/landing/src/Homepage.tsx | all | component | Function component. Renders: Platforms, UseCases, LlmReady, OpenSource, ClosingCta. |
| `apps/landing/src/Navbar::NavBar` | apps/landing/src/Navbar.tsx | all | component | Function component. Hooks: useState. Renders: nav, div, a, img, button, X, Menu. |
| `apps/landing/src/Pricing::CorporateBand` | apps/landing/src/Pricing.tsx | all | component | Function component. Props: tier. Renders: div, span, h3, p, a. |
| `apps/landing/src/Pricing::FAQ` | apps/landing/src/Pricing.tsx | all | component | Function component. Renders: div, h2, h3, p. |
| `apps/landing/src/Pricing::Pricing` | apps/landing/src/Pricing.tsx | all | component | Function component. Hooks: useState. Renders: div, PricingHeader, PricingCard, CorporateBand, FAQ. |
| `apps/landing/src/Pricing::PricingCard` | apps/landing/src/Pricing.tsx | all | component | Function component. Props: tier, billingPeriod. Renders: div, h3, p, span, ul, li, Check, ExternalLink. |
| `apps/landing/src/Pricing::PricingHeader` | apps/landing/src/Pricing.tsx | all | component | Function component. Props: billingPeriod, setBillingPeriod. Renders: div, span, h1, p, button. |
| `apps/landing/src/Privacy::PrivacyPolicy` | apps/landing/src/Privacy.tsx | all | component | Function component. Renders: div, main, h1, p, em, strong. |
| `apps/landing/src/Terms::Terms` | apps/landing/src/Terms.tsx | all | component | Function component. Renders: div, main, h1, p, em, strong. |
| `apps/mobile/app/+not-found::NotFound` | apps/mobile/app/+not-found.tsx | all | component | Function component. Renders: View. |
| `apps/mobile/app/dashboard/_layout::Dashboard` | apps/mobile/app/dashboard/_layout.tsx | all | component | Function component. Hooks: useRouter, useTranslation, useColorScheme, useIsLoggedIn, useEffect. Renders: Stack, Stack.Screen, BookmarkListHeader. |
| `apps/mobile/app/dashboard/(tabs)/_layout::TabLayout` | apps/mobile/app/dashboard/(tabs)/_layout.tsx | all | component | Function component. Hooks: useColorScheme, useTranslation. Renders: NativeTabs, NativeTabs.Trigger, NativeTabs.Trigger.Icon, NativeTabs.Trigger.VectorIcon, NativeTabs.Trigger.Label. |
| `apps/mobile/app/dashboard/(tabs)/(highlights)/_layout::Layout` | apps/mobile/app/dashboard/(tabs)/(highlights)/_layout.tsx | all | component | Function component. Hooks: useTranslation. Renders: Stack, ProfileAvatarButton, Stack.Screen. |
| `apps/mobile/app/dashboard/(tabs)/(highlights)/index::Highlights` | apps/mobile/app/dashboard/(tabs)/(highlights)/index.tsx | all | component | Function component. Hooks: useTRPC, useQueryClient, useInfiniteQuery. Renders: QueryPageState, HighlightList. |
| `apps/mobile/app/dashboard/(tabs)/(home)/_layout::Layout` | apps/mobile/app/dashboard/(tabs)/(home)/_layout.tsx | all | component | Function component. Hooks: useTranslation. Renders: Stack, BookmarkListHeader, Stack.Screen. |
| `apps/mobile/app/dashboard/(tabs)/(home)/index::Home` | apps/mobile/app/dashboard/(tabs)/(home)/index.tsx | all | component | Function component. Hooks: useTranslation, useColorScheme, useState, useNewBookmarkActions. Renders: InlineSearch, AndroidSearchBar, ProfileAvatarButton, BookmarkListHeader, UpdatingBookmarkList, ConnectionBanner. |
| `apps/mobile/app/dashboard/(tabs)/(lists)/_layout::Layout` | apps/mobile/app/dashboard/(tabs)/(lists)/_layout.tsx | all | component | Function component. Hooks: useTranslation. Renders: Stack, Stack.Screen. |
| `apps/mobile/app/dashboard/(tabs)/(lists)/index::ListRow` | apps/mobile/app/dashboard/(tabs)/(lists)/index.tsx | all | component | Function component. Props: item, onToggle. Hooks: useColorScheme, useTranslation. Renders: Pressable, View, Text, AppIcon, ChevronRight, GroupedListRow. |
| `apps/mobile/app/dashboard/(tabs)/(lists)/index::Lists` | apps/mobile/app/dashboard/(tabs)/(lists)/index.tsx | all | component | Function component. Hooks: useColorScheme, useTranslation, useSharedTranslation, useState, useBookmarkLists, useTRPC, +7 more. Renders: AppIcon, QueryPageState, Stack.Screen, View, Pressable, ProfileAvatarButton. |
| `apps/mobile/app/dashboard/(tabs)/(search)/_layout::Layout` | apps/mobile/app/dashboard/(tabs)/(search)/_layout.tsx | all | component | Function component. Hooks: useTranslation. Renders: Stack, Stack.Screen. |
| `apps/mobile/app/dashboard/(tabs)/(search)/index.ios::SearchTab` | apps/mobile/app/dashboard/(tabs)/(search)/index.ios.tsx | all | component | Function component. Hooks: useTranslation, useState, useRef, useBookmarkSearchState, useFocusEffect, useCallback. Renders: Stack.Screen, BookmarkSearchResults, SearchModeSelector. |
| `apps/mobile/app/dashboard/(tabs)/(tags)/_layout::Layout` | apps/mobile/app/dashboard/(tabs)/(tags)/_layout.tsx | all | component | Function component. Hooks: useTranslation. Renders: Stack, Stack.Screen. |
| `apps/mobile/app/dashboard/(tabs)/(tags)/index::Tags` | apps/mobile/app/dashboard/(tabs)/(tags)/index.tsx | all | component | Function component. Hooks: useTranslation, useState, useTRPC, useQueryClient, useColorScheme, useDebounce, +1 more. Renders: QueryPageState, Stack.Screen, View, Pressable, AppIcon, ProfileAvatarButton. |
| `apps/mobile/app/dashboard/(tabs)/index::TabIndex` | apps/mobile/app/dashboard/(tabs)/index.tsx | all | component | Function component. Renders: Redirect. |
| `apps/mobile/app/dashboard/archive::Archive` | apps/mobile/app/dashboard/archive.tsx | all | component | Function component. Hooks: useTranslation. Renders: UpdatingBookmarkList. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/highlights::BookmarkHighlightsPage` | apps/mobile/app/dashboard/bookmarks/[slug]/highlights.tsx | all | component | Function component. Hooks: useLocalSearchParams, useTRPC, useTranslation, useQueryClient, useQuery. Renders: QueryPageState, Stack.Screen, HeaderTextButton, HighlightList. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/index::BookmarkView` | apps/mobile/app/dashboard/bookmarks/[slug]/index.tsx | all | component | Function component. Hooks: useRouter, useLocalSearchParams, useColorScheme, useAppSettings, useConnectionStatus, useTranslation, +5 more. Renders: QueryPageState, BookmarkLinkView, BookmarkTextView, BookmarkAssetView, KeyboardAvoidingView, KeepScreenOn. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/index::SymbolOrAa` | apps/mobile/app/dashboard/bookmarks/[slug]/index.tsx | all | component | Function component. Props: color. Renders: SymbolView, ALargeSmall. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/info::AISummarySection` | apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx | all | component | Function component. Props: bookmark, readOnly. Hooks: useTranslation, useToast, useColorScheme, useState, useSummarizeBookmark, useUpdateBookmark. Renders: GroupedSection, Pressable, View, BookmarkTextMarkdown, Text, RowSeparator. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/info::BookmarkActionsSection` | apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx | all | component | Function component. Props: bookmark. Hooks: useTranslation, useCommonStrings, useToast, useAppSettings, useColorScheme, useUpdateBookmark, +1 more. Renders: GroupedSection, Pressable, View, AppIcon, Text, Switch. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/info::ManageListsRow` | apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx | all | component | Function component. Props: bookmark. Hooks: useTranslation, useTRPC, useQuery. Renders: NavigationRow. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/info::NotesEditor` | apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx | all | component | Function component. Props: notes, setNotes, isPending, disabled. Hooks: useTranslation, useColorScheme. Renders: GroupedSection, TextInput. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/info::TagList` | apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx | all | component | Function component. Props: bookmark, readOnly. Hooks: useTranslation. Renders: GroupedSection, View, Skeleton, TagPill, RowSeparator, NavigationRow. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/info::TitleEditor` | apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx | all | component | Function component. Props: title, setTitle, isPending, disabled. Hooks: useTranslation, useColorScheme. Renders: GroupedSection, TextInput. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/info::ViewBookmarkPage` | apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx | all | component | Arrow function component. Hooks: useHeaderHeight, useLocalSearchParams, useTranslation, useCommonActions, useToast, useWhoAmI, +5 more. Renders: QueryPageState, KeyboardGestureArea, Stack.Screen, Pressable, ActivityIndicator, Text. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/manage_lists::ListPickerPage` | apps/mobile/app/dashboard/bookmarks/[slug]/manage_lists.tsx | all | component | Arrow function component. Hooks: useHeaderHeight, useTRPC, useLocalSearchParams, useColorScheme, useTranslation, useCommonStrings, +7 more. Renders: QueryPageState, Stack.Screen, Link, Pressable, Plus, HeaderTextButton. |
| `apps/mobile/app/dashboard/bookmarks/[slug]/manage_tags::TagPickerPage` | apps/mobile/app/dashboard/bookmarks/[slug]/manage_tags.tsx | all | component | Arrow function component. Hooks: useHeaderHeight, useColorScheme, useLocalSearchParams, useState, useToast, useTranslation, +8 more. Renders: QueryPageState, Stack.Screen, HeaderTextButton, ScrollView, GroupedSection, React.Fragment. |
| `apps/mobile/app/dashboard/bookmarks/new::NoteEditorPage` | apps/mobile/app/dashboard/bookmarks/new.tsx | all | component | Arrow function component. Hooks: useState, useColorScheme, useTranslation, useCreateBookmark, useDiscardGuard. Renders: ScrollView, SheetHeader, Input, Text, View, HintIcon. |
| `apps/mobile/app/dashboard/favourites::Favourites` | apps/mobile/app/dashboard/favourites.tsx | all | component | Function component. Hooks: useTranslation. Renders: UpdatingBookmarkList. |
| `apps/mobile/app/dashboard/lists/[slug]/add::AddBookmarksToListPage` | apps/mobile/app/dashboard/lists/[slug]/add.tsx | all | component | Function component. Hooks: useLocalSearchParams, useTRPC, useColorScheme, useToast, useTranslation, useState, +6 more. Renders: QueryPageState, Stack.Screen, HeaderTextButton, FlatList, SearchInput, View. |
| `apps/mobile/app/dashboard/lists/[slug]/add::PickerThumbnail` | apps/mobile/app/dashboard/lists/[slug]/add.tsx | all | component | Function component. Props: bookmark. Hooks: useColorScheme, useAppSettings. Renders: View, AppIcon, Image. |
| `apps/mobile/app/dashboard/lists/[slug]/edit::EditListPage` | apps/mobile/app/dashboard/lists/[slug]/edit.tsx | all | component | Arrow function component. Hooks: useLocalSearchParams, useState, useToast, useTranslation, useCommonStrings, useTRPC, +4 more. Renders: QueryPageState, SheetHeader, FullPageSpinner, KeyboardAwareScrollView, ListFormFields, GroupedSection. |
| `apps/mobile/app/dashboard/lists/[slug]/index::ListActionsMenu` | apps/mobile/app/dashboard/lists/[slug]/index.tsx | all | component | Function component. Props: listId, name, canAdd, role, isLoaded. Hooks: useTRPC, useColorScheme, useTranslation, useCommonActions, useMenuIconColors, useBookmarkListLayoutMenu, +6 more. Renders: MenuView, Pressable, AppIcon. |
| `apps/mobile/app/dashboard/lists/[slug]/index::ListView` | apps/mobile/app/dashboard/lists/[slug]/index.tsx | all | component | Function component. Hooks: useLocalSearchParams, useTranslation, useTRPC, useQuery, useArchiveFilter. Renders: Stack.Screen, ListActionsMenu, QueryPageState, UpdatingBookmarkList, FullPageSpinner. |
| `apps/mobile/app/dashboard/lists/[slug]/sharing::ListSharingPage` | apps/mobile/app/dashboard/lists/[slug]/sharing.tsx | all | component | Function component. Hooks: useLocalSearchParams, useTranslation, useTRPC, useQuery. Renders: Stack.Screen, Pressable, Text, KeyboardAwareScrollView, ListSharingSettings, QueryPageState. |
| `apps/mobile/app/dashboard/lists/new::NewListPage` | apps/mobile/app/dashboard/lists/new.tsx | all | component | Arrow function component. Hooks: useLocalSearchParams, useToast, useTranslation, useCommonStrings, useState, useEffect, +3 more. Renders: KeyboardAwareScrollView, SheetHeader, SegmentedControl, Text, ListFormFields. |
| `apps/mobile/app/dashboard/lists/select-parent::SelectListParentPage` | apps/mobile/app/dashboard/lists/select-parent.tsx | all | component | Function component. Hooks: useLocalSearchParams, useTranslation, useCommonActions, useState, useBookmarkLists, useMemo. Renders: QueryPageState, Stack.Screen, HeaderTextButton, ScrollView, ListPicker. |
| `apps/mobile/app/dashboard/settings/_layout::SettingsLayout` | apps/mobile/app/dashboard/settings/_layout.tsx | all | component | Function component. Hooks: useColorScheme, useTranslation. Renders: Stack, HeaderTextButton, Stack.Screen. |
| `apps/mobile/app/dashboard/settings/bookmark-default-view::BookmarkDefaultViewSettings` | apps/mobile/app/dashboard/settings/bookmark-default-view.tsx | all | component | Function component. Hooks: useRouter, useToast, useAppSettings, useTranslation, useCommonStrings. Renders: SettingsScreen, SettingsGroup, View, SettingsSeparator, SettingsChoiceRow. |
| `apps/mobile/app/dashboard/settings/index::Settings` | apps/mobile/app/dashboard/settings/index.tsx | all | component | Function component. Hooks: useRouter, useTRPC, useSession, useAppSettings, useTranslation, useCommonActions, +7 more. Renders: SettingsScreen, UserProfileHeader, SettingsGroup, SettingsNavigationRow, SettingsSeparator, SettingsValueRow. |
| `apps/mobile/app/dashboard/settings/language::LanguagePage` | apps/mobile/app/dashboard/settings/language.tsx | all | component | Function component. Hooks: useAppSettings, useTranslation. Renders: SettingsScreen, SettingsGroup, View, SettingsSeparator, SettingsChoiceRow. |
| `apps/mobile/app/dashboard/settings/offline-articles::OfflineArticles` | apps/mobile/app/dashboard/settings/offline-articles.tsx | all | component | Function component. Hooks: useRouter, useHeaderHeight, useAppSettings, useTranslation, useCommonActions, useColorScheme, +2 more. Renders: FlashList, View, EmptyState, Pressable, Text, Trash2. |
| `apps/mobile/app/dashboard/settings/offline-lists::OfflineLists` | apps/mobile/app/dashboard/settings/offline-lists.tsx | all | component | Function component. Hooks: useAppSettings, useTranslation, useOfflineDownloadPrefs, useBookmarkLists, useMemo. Renders: QueryPageState, SettingsScreen, Text, ListPicker. |
| `apps/mobile/app/dashboard/settings/offline::DownloadProgress` | apps/mobile/app/dashboard/settings/offline.tsx | all | component | Function component. Props: status. Renders: View. |
| `apps/mobile/app/dashboard/settings/offline::OfflineContent` | apps/mobile/app/dashboard/settings/offline.tsx | all | component | Function component. Hooks: useRouter, useQueryClient, useToast, useTranslation, useCommonActions, useAppSettings, +4 more. Renders: SettingsScreen, Text, SettingsGroup, SettingsToggleRow, SettingsSeparator, SettingsMenuRow. |
| `apps/mobile/app/dashboard/settings/offline::SectionHeader` | apps/mobile/app/dashboard/settings/offline.tsx | all | component | Function component. Props: title, detail. Renders: View, Text. |
| `apps/mobile/app/dashboard/settings/reader-settings::ReaderSettingsPage` | apps/mobile/app/dashboard/settings/reader-settings.tsx | all | component | Function component. Hooks: useTranslation, useReaderSettings, useState, useRef, useCallback, useEffect. Renders: SettingsScreen, View, Text, SettingsGroup, SettingsSeparator, SettingsChoiceRow. |
| `apps/mobile/app/dashboard/settings/reading::ReaderViewSettings` | apps/mobile/app/dashboard/settings/reading.tsx | all | component | Function component. Hooks: useRouter, useAppSettings, useTranslation. Renders: SettingsScreen, SettingsGroup, SettingsNavigationRow, SettingsSeparator, SettingsToggleRow. |
| `apps/mobile/app/dashboard/settings/subscription::SubscriptionSettings` | apps/mobile/app/dashboard/settings/subscription.tsx | all | component | Function component. Hooks: useTRPC, useQueryClient, useToast, useTranslation, useSharedTranslation, useInAppPurchases, +3 more. Renders: SettingsScreen, SettingsGroup, SettingsValueRow, SettingsSeparator, SettingsActionRow. |
| `apps/mobile/app/dashboard/settings/theme::ThemePage` | apps/mobile/app/dashboard/settings/theme.tsx | all | component | Function component. Hooks: useAppSettings, useTranslation. Renders: SettingsScreen, SettingsGroup, View, SettingsSeparator, SettingsChoiceRow. |
| `apps/mobile/app/dashboard/settings/toolbar-settings::ToolbarSettingsPage` | apps/mobile/app/dashboard/settings/toolbar-settings.tsx | all | component | Function component. Hooks: useAppSettings, useTranslation, useToolbarActionLabels, useCallback. Renders: ScaleDecorator, Pressable, TailwindResolver, GripVertical, AppIcon, Text. |
| `apps/mobile/app/dashboard/settings/uploads::UploadSettings` | apps/mobile/app/dashboard/settings/uploads.tsx | all | component | Function component. Hooks: useAppSettings, useTranslation. Renders: SettingsScreen, SettingsGroup, View, SettingsSeparator, SettingsChoiceRow. |
| `apps/mobile/app/dashboard/tags/[slug]::TagActionsMenu` | apps/mobile/app/dashboard/tags/[slug].tsx | all | component | Function component. Props: tagId, tagName. Hooks: useColorScheme, useMenuIconColors, useBookmarkListLayoutMenu, useToast, useTranslation, useCommonActions, +1 more. Renders: MenuView, View, Pressable, AppIcon. |
| `apps/mobile/app/dashboard/tags/[slug]::TagView` | apps/mobile/app/dashboard/tags/[slug].tsx | all | component | Function component. Hooks: useLocalSearchParams, useTranslation, useTRPC, useQuery, useArchiveFilter. Renders: Stack.Screen, TagActionsMenu, QueryPageState, UpdatingBookmarkList, FullPageSpinner. |
| `apps/mobile/app/dashboard/tags/[slug]/edit::EditTagPage` | apps/mobile/app/dashboard/tags/[slug]/edit.tsx | all | component | Function component. Hooks: useLocalSearchParams, useState, useTRPC, useToast, useTranslation, useCommonStrings, +4 more. Renders: QueryPageState, FullPageSpinner, ScrollView, SheetHeader, Input, Text. |
| `apps/mobile/app/dashboard/tags/new::NewTagPage` | apps/mobile/app/dashboard/tags/new.tsx | all | component | Function component. Hooks: useState, useToast, useTranslation, useCreateTag, useDiscardGuard. Renders: ScrollView, SheetHeader, Input, Text. |
| `apps/mobile/app/error::ErrorPage` | apps/mobile/app/error.tsx | all | component | Function component. Hooks: useTranslation. Renders: View, Text. |
| `apps/mobile/app/index::App` | apps/mobile/app/index.tsx | all | component | Function component. Hooks: useIsLoggedIn. Renders: FullPageSpinner, Redirect. |
| `apps/mobile/app/server-address::ServerAddress` | apps/mobile/app/server-address.tsx | all | component | Function component. Hooks: useRouter, useTranslation, useCommonStrings, useColorScheme, useAppSettings, useState, +1 more. Renders: KeyboardAwareScrollView, SheetHeader, View, GroupedSection, Input, Text. |
| `apps/mobile/app/sharing::Sharing` | apps/mobile/app/sharing.tsx | all | component | Function component. Hooks: useRouter, useTranslation, useState, useRef, useEffect. Renders: View, SaveBookmark, LoadingAnimation, Animated.View, Text, Pressable. |
| `apps/mobile/app/signin::FieldRow` | apps/mobile/app/signin.tsx | all | component | Wrapped component. Props: label, ...props. Renders: View, Text, TextInput. |
| `apps/mobile/app/signin::Signin` | apps/mobile/app/signin.tsx | all | component | Function component. Hooks: useAppSettings, useTranslation, useRouter, useTRPC, useState, useLoginErrorMessage, +2 more. Renders: Redirect, KeyboardAwareScrollView, View, TailwindResolver, Logo, GroupedSection. |
| `apps/mobile/app/test-connection::TestConnection` | apps/mobile/app/test-connection.tsx | all | component | Function component. Hooks: useAppSettings, useTranslation, useColorScheme, useToast, useState, useEffect. Renders: ScrollView, Stack.Screen, HeaderTextButton, GroupedSection, View, ActivityIndicator. |
| `apps/mobile/components/bookmarks/AttachmentBox::AttachmentBox` | apps/mobile/components/bookmarks/AttachmentBox.tsx | all | component | Function component. Props: bookmark. Hooks: useAppSettings, useColorScheme, useToast, useTranslation, useSharedTranslation, useState, +1 more. Renders: GroupedSection, Text, Fragment, RowSeparator, Pressable, Icon. |
| `apps/mobile/components/bookmarks/BookmarkAssetImage::BookmarkAssetImage` | apps/mobile/components/bookmarks/BookmarkAssetImage.tsx | all | component | Function component. Props: assetId, className, contentFit, contentPosition. Hooks: useAssetUrl. Renders: View, Image. |
| `apps/mobile/components/bookmarks/BookmarkAssetView::BookmarkAssetView` | apps/mobile/components/bookmarks/BookmarkAssetView.tsx | all | component | Function component. Props: bookmark. Hooks: useState, useAssetUrl. Renders: View, PDFViewer, ImageView, Pressable, BookmarkAssetImage. |
| `apps/mobile/components/bookmarks/BookmarkCard::BookmarkCard` | apps/mobile/components/bookmarks/BookmarkCard.tsx | all | component | Function component. Props: bookmark. Hooks: useTRPC, useQuery, useRouter, useAppSettings, useToast, useTranslation, +5 more. Renders: CardGestures, CardActions, Layout. |
| `apps/mobile/components/bookmarks/BookmarkCard::BookmarkFooterMetadata` | apps/mobile/components/bookmarks/BookmarkCard.tsx | all | component | Function component. Props: ctx. Hooks: useColorScheme, useTranslation. Renders: View, BookmarkCardContainer.FooterExtras, Text, AppIcon. |
| `apps/mobile/components/bookmarks/BookmarkCard::CardActions` | apps/mobile/components/bookmarks/BookmarkCard.tsx | all | component | Function component. Props: actions, compact, itemName. Renders: View, ActionBar. |
| `apps/mobile/components/bookmarks/BookmarkCard::CardGestures` | apps/mobile/components/bookmarks/BookmarkCard.tsx | all | component | Function component. Props: actions, label, href, onOpen, overlay, children. Hooks: useTranslation, useRef. Renders: Pressable, BookmarkCardContainer.Root, Link, Link.Trigger, Link.Menu, ReanimatedSwipeable. |
| `apps/mobile/components/bookmarks/BookmarkCard::CardLayout` | apps/mobile/components/bookmarks/BookmarkCard.tsx | all | component | Function component. Props: ctx. Renders: BookmarkCardContainer.Provider, BookmarkCardContainer.Media, View, BookmarkCardContainer.Title, BookmarkFooterMetadata, BookmarkCardContainer.Body. |
| `apps/mobile/components/bookmarks/BookmarkCard::ExpandedLinkImage` | apps/mobile/components/bookmarks/BookmarkCard.tsx | all | component | Function component. Props: source. Hooks: useState. Renders: View, Image. |
| `apps/mobile/components/bookmarks/BookmarkCard::LinkPlaceholder` | apps/mobile/components/bookmarks/BookmarkCard.tsx | all | component | Function component. Props: iconSize. Hooks: useColorScheme. Renders: View, AppIcon. |
| `apps/mobile/components/bookmarks/BookmarkCard::ListLayout` | apps/mobile/components/bookmarks/BookmarkCard.tsx | all | component | Function component. Props: ctx. Hooks: useAppSettings. Renders: BookmarkCardContainer.Provider, View, BookmarkCardContainer.CompactMedia, Text, BookmarkFooterMetadata, BookmarkCardContainer.CompactBody. |
| `apps/mobile/components/bookmarks/BookmarkCard::SwipeAction` | apps/mobile/components/bookmarks/BookmarkCard.tsx | all | component | Function component. Props: icon, label, className, align. Renders: View, AppIcon, Text. |
| `apps/mobile/components/bookmarks/BookmarkContentLoading::BookmarkContentLoading` | apps/mobile/components/bookmarks/BookmarkContentLoading.tsx | all | component | Function component. Hooks: useRef, useEffect. Renders: View, Animated.View, Globe, Text. |
| `apps/mobile/components/bookmarks/BookmarkHtmlHighlighterDom::BookmarkHtmlHighlighterDom` | apps/mobile/components/bookmarks/BookmarkHtmlHighlighterDom.tsx | all | component | Function component. Props: htmlContent, contentStyle, isDark, highlights, readOnly, onHighlight, +17 more. Hooks: useRef, useEffect. Renders: div, style, h1, p, ScrollProgressTracker, BookmarkHTMLHighlighter. |
| `apps/mobile/components/bookmarks/BookmarkLinkPreview::BookmarkLinkArchivePreview` | apps/mobile/components/bookmarks/BookmarkLinkPreview.tsx | all | component | Function component. Props: bookmark. Hooks: useTranslation, useAssetUrl, useCallback. Renders: View, Text, WebView. |
| `apps/mobile/components/bookmarks/BookmarkLinkPreview::BookmarkLinkBrowserPreview` | apps/mobile/components/bookmarks/BookmarkLinkPreview.tsx | all | component | Function component. Props: bookmark. Hooks: useCallback. Renders: WebView. |
| `apps/mobile/components/bookmarks/BookmarkLinkPreview::BookmarkLinkPdfPreview` | apps/mobile/components/bookmarks/BookmarkLinkPreview.tsx | all | component | Function component. Props: bookmark. Hooks: useTranslation, useAssetUrl. Renders: View, Text, PDFViewer. |
| `apps/mobile/components/bookmarks/BookmarkLinkPreview::BookmarkLinkReaderPreview` | apps/mobile/components/bookmarks/BookmarkLinkPreview.tsx | all | component | Function component. Props: bookmark. Hooks: useTranslation, useCommonActions, useColorScheme, useLocalSearchParams, useSafeAreaInsets, useReaderSettings, +16 more. Renders: QueryPageState, View, Stack.Screen, ImageView, BookOpen, Text. |
| `apps/mobile/components/bookmarks/BookmarkLinkPreview::BookmarkLinkScreenshotPreview` | apps/mobile/components/bookmarks/BookmarkLinkPreview.tsx | all | component | Function component. Props: bookmark. Hooks: useTranslation, useAssetUrl, useState. Renders: View, Text, ImageView, ScrollView, Pressable, Image. |
| `apps/mobile/components/bookmarks/BookmarkLinkTypeSelector::BookmarkLinkTypeSelector` | apps/mobile/components/bookmarks/BookmarkLinkTypeSelector.tsx | all | component | Function component. Props: type, onChange, bookmark. Hooks: useTranslation, useMenuIconColors, useColorScheme. Renders: MenuView, Pressable, Text, ChevronDown. |
| `apps/mobile/components/bookmarks/BookmarkLinkView::BookmarkLinkView` | apps/mobile/components/bookmarks/BookmarkLinkView.tsx | all | component | Function component. Props: bookmark, bookmarkPreviewType. Renders: BookmarkContentLoading, BookmarkLinkBrowserPreview, BookmarkLinkReaderPreview, BookmarkLinkScreenshotPreview, BookmarkLinkArchivePreview, BookmarkLinkPdfPreview. |
| `apps/mobile/components/bookmarks/BookmarkList::BookmarkList` | apps/mobile/components/bookmarks/BookmarkList.tsx | all | component | Function component. Props: bookmarks, header, onRefresh, fetchNextPage, isFetchingNextPage, isRefreshing, +2 more. Hooks: useRef, useTranslation, useScrollToTop, useAppSettings, useTRPC, useMutationState, +2 more. Renders: View, Animated.FlatList, BookmarkCard, EmptyState, ActivityIndicator. |
| `apps/mobile/components/bookmarks/BookmarkListHeader::BookmarkListHeader` | apps/mobile/components/bookmarks/BookmarkListHeader.tsx | all | component | Function component. Hooks: useBookmarkListLayoutMenu, useColorScheme, useTranslation. Renders: MenuView, View, AppIcon. |
| `apps/mobile/components/bookmarks/BookmarkTextMarkdown::BookmarkTextMarkdown` | apps/mobile/components/bookmarks/BookmarkTextMarkdown.tsx | all | component | Function component. Props: text, size, muted. Renders: TailwindResolver, Markdown. |
| `apps/mobile/components/bookmarks/BookmarkTextView::BookmarkTextView` | apps/mobile/components/bookmarks/BookmarkTextView.tsx | all | component | Function component. Props: bookmark. Hooks: useToast, useTranslation, useCommonActions, useColorScheme, useState, useDiscardGuard, +1 more. Renders: View, Stack.Screen, HeaderTextButton, TextInput, ScrollView, Text. |
| `apps/mobile/components/bookmarks/BottomActions::BottomActions` | apps/mobile/components/bookmarks/BottomActions.tsx | all | component | Function component. Props: bookmark. Hooks: useToolbarActions, useSafeAreaInsets, useRouter, useToast, useTranslation, useCommonActions, +1 more. Renders: View, ToolbarContainer, Pressable, ToolbarItem, MenuView, TailwindResolver. |
| `apps/mobile/components/bookmarks/BottomActions::ToolbarContainer` | apps/mobile/components/bookmarks/BottomActions.tsx | all | component | Function component. Props: children, bottomMargin, bottomInset. Renders: View, GlassView, BlurView. |
| `apps/mobile/components/bookmarks/BottomActions::ToolbarItem` | apps/mobile/components/bookmarks/BottomActions.tsx | all | component | Function component. Props: icon, label, showLabel. Renders: View, Text. |
| `apps/mobile/components/bookmarks/card/ActionBar::ActionBar` | apps/mobile/components/bookmarks/card/ActionBar.tsx | all | component | Function component. Props: actions, compact, itemName. Hooks: useTranslation, useColorScheme. Renders: View, ActivityIndicator, Pressable, AppIcon, MenuView. |
| `apps/mobile/components/bookmarks/card/BookmarkCard::Body` | apps/mobile/components/bookmarks/card/BookmarkCard.tsx | all | component | Function component. Hooks: useContext. Renders: PressableSlot. |
| `apps/mobile/components/bookmarks/card/BookmarkCard::CompactBody` | apps/mobile/components/bookmarks/card/BookmarkCard.tsx | all | component | Function component. Hooks: useContext. Renders: PressableSlot. |
| `apps/mobile/components/bookmarks/card/BookmarkCard::CompactMedia` | apps/mobile/components/bookmarks/card/BookmarkCard.tsx | all | component | Function component. Hooks: useContext. Renders: PressableSlot. |
| `apps/mobile/components/bookmarks/card/BookmarkCard::FooterExtras` | apps/mobile/components/bookmarks/card/BookmarkCard.tsx | all | component | Function component. Hooks: useContext. Renders: View. |
| `apps/mobile/components/bookmarks/card/BookmarkCard::Media` | apps/mobile/components/bookmarks/card/BookmarkCard.tsx | all | component | Function component. Hooks: useContext. Renders: PressableSlot. |
| `apps/mobile/components/bookmarks/card/BookmarkCard::NoteSection` | apps/mobile/components/bookmarks/card/BookmarkCard.tsx | all | component | Function component. Hooks: useAppSettings, useContext. Renders: NotePreview. |
| `apps/mobile/components/bookmarks/card/BookmarkCard::PressableSlot` | apps/mobile/components/bookmarks/card/BookmarkCard.tsx | all | component | Function component. Props: children, onPress. Renders: Pressable. |
| `apps/mobile/components/bookmarks/card/BookmarkCard::Root` | apps/mobile/components/bookmarks/card/BookmarkCard.tsx | all | component | Function component. Props: children. Renders: View. |
| `apps/mobile/components/bookmarks/card/BookmarkCard::Title` | apps/mobile/components/bookmarks/card/BookmarkCard.tsx | all | component | Function component. Hooks: useContext. Renders: Text. |
| `apps/mobile/components/bookmarks/card/TagList::TagList` | apps/mobile/components/bookmarks/card/TagList.tsx | all | component | Function component. Props: bookmark, maxVisible. Hooks: useTranslation, useWhoAmI. Renders: TagListSkeleton, View, TagPill, Text. |
| `apps/mobile/components/bookmarks/card/TagList::TagListSkeleton` | apps/mobile/components/bookmarks/card/TagList.tsx | all | component | Function component. Renders: View, Skeleton. |
| `apps/mobile/components/bookmarks/NotePreview::NotePreview` | apps/mobile/components/bookmarks/NotePreview.tsx | all | component | Function component. Props: note, bookmarkId, readOnly. Hooks: useState, useTranslation, useColorScheme. Renders: Pressable, View, AppIcon, Text, Modal, X. |
| `apps/mobile/components/bookmarks/PDFViewer::PDFViewer` | apps/mobile/components/bookmarks/PDFViewer.tsx | all | component | Function component. Props: source, headers. Hooks: useState, useTranslation, useColorScheme, useQuery, useMemo, useEffect. Renders: View, Text, ActivityIndicator, Pdf. |
| `apps/mobile/components/bookmarks/TagPill::TagPill` | apps/mobile/components/bookmarks/TagPill.tsx | all | component | Function component. Props: tag, clickable. Renders: View, Text, Link, Pressable. |
| `apps/mobile/components/bookmarks/UpdatingBookmarkList::UpdatingBookmarkList` | apps/mobile/components/bookmarks/UpdatingBookmarkList.tsx | all | component | Function component. Props: query, header, emptyState, scrollToTopOnSave. Hooks: useTRPC, useQueryClient, useAppSettings, useInfiniteQuery. Renders: QueryPageState, BookmarkList. |
| `apps/mobile/components/ConnectionBanner::ConnectionBanner` | apps/mobile/components/ConnectionBanner.tsx | all | component | Function component. Hooks: useConnectionStatus, useColorScheme, useTranslation. Renders: View, Icon, Text. |
| `apps/mobile/components/ConnectionStatusIndicator::ConnectionStatusIndicator` | apps/mobile/components/ConnectionStatusIndicator.tsx | all | component | Function component. Hooks: useConnectionStatus, useTranslation. Renders: View, CloudOff. |
| `apps/mobile/components/CustomHeadersModal::CustomHeadersModal` | apps/mobile/components/CustomHeadersModal.tsx | all | component | Function component. Props: visible, customHeaders, onClose, onSave. Hooks: useTranslation, useCommonActions, useColorScheme, useState. Renders: Modal, View, Pressable, KeyboardAwareScrollView, Text, X. |
| `apps/mobile/components/FullPageError::FullPageError` | apps/mobile/components/FullPageError.tsx | all | component | Function component. Props: error, onRetry, secondaryLabel, onSecondary, title, icon, +1 more. Hooks: useColorScheme, useTranslation. Renders: View, AppIcon, Text, Button. |
| `apps/mobile/components/highlights/HighlightCard::HighlightCard` | apps/mobile/components/highlights/HighlightCard.tsx | all | component | Function component. Props: highlight. Hooks: useToast, useTranslation, useCommonActions, useCommonStrings, useRouter, useTRPC, +4 more. Renders: View, Pressable, Text, AppIcon, ActivityIndicator, MenuView. |
| `apps/mobile/components/highlights/HighlightList::HighlightList` | apps/mobile/components/highlights/HighlightList.tsx | all | component | Function component. Props: highlights, header, onRefresh, fetchNextPage, isFetchingNextPage, isRefreshing. Hooks: useTranslation, useContainerWidth. Renders: View, Animated.FlatList, HighlightCard, EmptyState, ActivityIndicator. |
| `apps/mobile/components/lists/list-parent-field::ListParentField` | apps/mobile/components/lists/list-parent-field.tsx | all | component | Function component. Props: value, onPress. Hooks: useTranslation, useBookmarkLists. Renders: Pressable, Text, ActivityIndicator, ChevronRight. |
| `apps/mobile/components/lists/list-picker::ListPicker` | apps/mobile/components/lists/list-picker.tsx | all | component | Function component. Props: options, onSelect, emptyMessage, singleChoice. Hooks: useColorScheme, useTranslation. Renders: View, Text, RowSeparator, Pressable, ActivityIndicator, Check. |
| `apps/mobile/components/lists/list-sharing-settings::ListSharingSettings` | apps/mobile/components/lists/list-sharing-settings.tsx | all | component | Function component. Props: list. Hooks: useTRPC, useQueryClient, useToast, useColorScheme, useAppSettings, useTranslation, +6 more. Renders: View, Text, GroupedSection, Globe, ActivityIndicator, Switch. |
| `apps/mobile/components/lists/list-sharing-settings::Person` | apps/mobile/components/lists/list-sharing-settings.tsx | all | component | Function component. Props: name, email, subtitle, children. Hooks: useTranslation. Renders: View, Text. |
| `apps/mobile/components/lists/list-sharing-settings::RolePicker` | apps/mobile/components/lists/list-sharing-settings.tsx | all | component | Function component. Props: role, onChange, disabled, label. Hooks: useColorScheme, useTranslation. Renders: MenuView, View, Text, ChevronDown. |
| `apps/mobile/components/lists/ListFormFields::ListFormFields` | apps/mobile/components/lists/ListFormFields.tsx | all | component | Function component. Props: name, onNameChange, icon, onIconChange, parentId, onPressParent, +5 more. Hooks: useTranslation, useRef, useTagAutocomplete. Renders: GroupedSection, View, EmojiPicker, Input, RowSeparator, ListParentField. |
| `apps/mobile/components/lists/pending-list-invitations::InvitationRow` | apps/mobile/components/lists/pending-list-invitations.tsx | all | component | Function component. Props: invitation. Hooks: useTRPC, useQueryClient, useToast, useTranslation, useSharedTranslation, useMutation. Renders: View, Text, Button, ActivityIndicator. |
| `apps/mobile/components/lists/pending-list-invitations::PendingListInvitations` | apps/mobile/components/lists/pending-list-invitations.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQuery. Renders: View, Text, InvitationRow. |
| `apps/mobile/components/Logo::Logo` | apps/mobile/components/Logo.tsx | all | component | Arrow function component. Props: props: SvgProps. Renders: Svg, Path, G. |
| `apps/mobile/components/navigation/stack::StackImpl` | apps/mobile/components/navigation/stack.tsx | all | component | Function component. Props: contentStyle, headerStyle, ...props. Renders: Stack. |
| `apps/mobile/components/QueryPageState::QueryPageState` | apps/mobile/components/QueryPageState.tsx | all | component | Function component. Props: error, onRetry. Hooks: useConnectionStatus, useTranslation, useAppSettings, useRouter, useSession. Renders: FullPageError, FullPageSpinner. |
| `apps/mobile/components/reader/ReaderPreview::ReaderPreview` | apps/mobile/components/reader/ReaderPreview.tsx | all | component | Wrapped component. Props: initialFontFamily, initialFontSize, initialLineHeight. Hooks: useRef, useColorScheme, useTranslation, useImperativeHandle, useEffect. Renders: View, WebView. |
| `apps/mobile/components/search/BookmarkSearchResults::BookmarkSearchResults` | apps/mobile/components/search/BookmarkSearchResults.tsx | all | component | Function component. Props: rawSearch, state, onSelectHistory, header. Hooks: useTranslation. Renders: View, GroupedListRow, Pressable, Text, FlatList, EmptyState. |
| `apps/mobile/components/search/InlineSearch::InlineSearch` | apps/mobile/components/search/InlineSearch.tsx | all | component | Function component. Props: onClose, rightElement. Hooks: useState, useRef, useSafeAreaInsets, useTranslation, useBookmarkSearchState. Renders: View, SearchInput, Pressable, TailwindResolver, XIcon, SearchModeSelector. |
| `apps/mobile/components/search/SearchModeSelector::SearchModeSelector` | apps/mobile/components/search/SearchModeSelector.tsx | all | component | Function component. Props: value, onValueChange, className. Hooks: useClientConfig, useTranslation, useMenuIconColors. Renders: View, MenuView, Pressable, TailwindResolver, ActiveIcon, Text. |
| `apps/mobile/components/settings/ProfileAvatarButton::ProfileAvatarButton` | apps/mobile/components/settings/ProfileAvatarButton.tsx | all | component | Function component. Hooks: useRouter, useTranslation, useTRPC, useQuery. Renders: Pressable, Avatar, ConnectionStatusIndicator. |
| `apps/mobile/components/settings/settings-list::SettingsActionRow` | apps/mobile/components/settings/settings-list.tsx | all | component | Function component. Props: centered, disabled, isLoading, label, leading, onPress, +1 more. Renders: Pressable, ActivityIndicator, Text. |
| `apps/mobile/components/settings/settings-list::SettingsChoiceRow` | apps/mobile/components/settings/settings-list.tsx | all | component | Function component. Props: description, disabled, label, labelStyle, onPress, selected. Hooks: useColorScheme. Renders: Pressable, View, Text, Check. |
| `apps/mobile/components/settings/settings-list::SettingsGroup` | apps/mobile/components/settings/settings-list.tsx | all | component | Function component. Props: children, footer, header. Renders: View, Text. |
| `apps/mobile/components/settings/settings-list::SettingsMenuRow` | apps/mobile/components/settings/settings-list.tsx | all | component | Function component. Props: label, onSelect, options, value. Hooks: useColorScheme. Renders: MenuView, View, Text, ChevronsUpDown. |
| `apps/mobile/components/settings/settings-list::SettingsNavigationRow` | apps/mobile/components/settings/settings-list.tsx | all | component | Function component. Props: isLoading, label, onPress, value. Renders: Pressable, Text, ActivityIndicator, ChevronRight. |
| `apps/mobile/components/settings/settings-list::SettingsScreen` | apps/mobile/components/settings/settings-list.tsx | all | component | Function component. Props: children, contentContainerStyle, ...props. Hooks: useHeaderHeight. Renders: ScrollView. |
| `apps/mobile/components/settings/settings-list::SettingsSeparator` | apps/mobile/components/settings/settings-list.tsx | all | component | Function component. Props: className, style. Renders: View. |
| `apps/mobile/components/settings/settings-list::SettingsToggleRow` | apps/mobile/components/settings/settings-list.tsx | all | component | Function component. Props: disabled, label, onValueChange, value. Renders: View, Text, Switch. |
| `apps/mobile/components/settings/settings-list::SettingsValueRow` | apps/mobile/components/settings/settings-list.tsx | all | component | Function component. Props: label, value. Renders: View, Text. |
| `apps/mobile/components/settings/UsageStatsScreen::ActivityCharts` | apps/mobile/components/settings/UsageStatsScreen.tsx | all | component | Function component. Props: stats. Hooks: useColorScheme, useTranslation. Renders: View, Text. |
| `apps/mobile/components/settings/UsageStatsScreen::MetricTile` | apps/mobile/components/settings/UsageStatsScreen.tsx | all | component | Function component. Props: label, value, icon, width. Hooks: useColorScheme. Renders: View, AppIcon, Text. |
| `apps/mobile/components/settings/UsageStatsScreen::ProgressRow` | apps/mobile/components/settings/UsageStatsScreen.tsx | all | component | Function component. Props: label, value, total, icon, color, detail, +1 more. Hooks: useColorScheme. Renders: View, Icon, Text. |
| `apps/mobile/components/settings/UsageStatsScreen::RankedList` | apps/mobile/components/settings/UsageStatsScreen.tsx | all | component | Function component. Props: items, emptyText. Renders: Text, View. |
| `apps/mobile/components/settings/UsageStatsScreen::SectionCard` | apps/mobile/components/settings/UsageStatsScreen.tsx | all | component | Function component. Props: title, icon, children. Hooks: useColorScheme. Renders: View, AppIcon, Text, SettingsSeparator. |
| `apps/mobile/components/settings/UsageStatsScreen::SectionLabel` | apps/mobile/components/settings/UsageStatsScreen.tsx | all | component | Function component. Props: children. Renders: Text. |
| `apps/mobile/components/settings/UsageStatsScreen::SourcesList` | apps/mobile/components/settings/UsageStatsScreen.tsx | all | component | Function component. Props: stats. Hooks: useColorScheme, useTranslation. Renders: Text, View, Icon. |
| `apps/mobile/components/settings/UsageStatsScreen::StatsSkeleton` | apps/mobile/components/settings/UsageStatsScreen.tsx | all | component | Function component. Renders: SettingsScreen, View, Skeleton. |
| `apps/mobile/components/settings/UsageStatsScreen::UsageStatsScreen` | apps/mobile/components/settings/UsageStatsScreen.tsx | all | component | Function component. Hooks: useWindowDimensions, useColorScheme, useTranslation, useTRPC, useQuery. Renders: StatsSkeleton, QueryPageState, SettingsScreen, RefreshControl, View, Text. |
| `apps/mobile/components/settings/UserProfileHeader::UserProfileHeader` | apps/mobile/components/settings/UserProfileHeader.tsx | all | component | Function component. Props: image, name, email. Hooks: useTranslation. Renders: View, Avatar, Text. |
| `apps/mobile/components/sharing/ErrorAnimation::ErrorAnimation` | apps/mobile/components/sharing/ErrorAnimation.tsx | all | component | Function component. Hooks: useSharedValue, useEffect, useAnimatedStyle. Renders: Animated.View, View, AlertCircle. |
| `apps/mobile/components/sharing/LoadingAnimation::LoadingAnimation` | apps/mobile/components/sharing/LoadingAnimation.tsx | all | component | Function component. Hooks: useSharedValue, useEffect, useAnimatedStyle. Renders: Animated.View, Archive, View, Text, Animated.Text. |
| `apps/mobile/components/sharing/SuccessAnimation::Particle` | apps/mobile/components/sharing/SuccessAnimation.tsx | all | component | Function component. Props: angle, delay, color. Hooks: useSharedValue, useEffect, useAnimatedStyle. Renders: Animated.View. |
| `apps/mobile/components/sharing/SuccessAnimation::SuccessAnimation` | apps/mobile/components/sharing/SuccessAnimation.tsx | all | component | Function component. Hooks: useSharedValue, useEffect, useAnimatedStyle. Renders: View, Particle, Animated.View, Check. |
| `apps/mobile/components/ui/ActionButton::ActionButton` | apps/mobile/components/ui/ActionButton.tsx | all | component | Function component. Props: children, loading, disabled, ...props. Renders: Pressable, ActivityIndicator. |
| `apps/mobile/components/ui/AndroidSearchBar::AndroidSearchBar` | apps/mobile/components/ui/AndroidSearchBar.tsx | all | component | Function component. Props: label, onPress, rightElement, trailingElement. Hooks: useSafeAreaInsets, useIsFocused. Renders: View, Pressable, TailwindResolver, Search, Text. |
| `apps/mobile/components/ui/AppIcon::AppIcon` | apps/mobile/components/ui/AppIcon.tsx | all | component | Function component. Props: icon, size, color, filled, accessibilityLabel. Renders: SymbolView, Icon. |
| `apps/mobile/components/ui/AppIcon::SelectionIndicator` | apps/mobile/components/ui/AppIcon.tsx | all | component | Function component. Props: selected, selectedColor, color. Renders: AppIcon. |
| `apps/mobile/components/ui/Avatar::Avatar` | apps/mobile/components/ui/Avatar.tsx | all | component | Function component. Props: image, name, size, className, fallbackClassName. Hooks: useState, useAssetUrl, useMemo, useEffect. Renders: View, Text, Image. |
| `apps/mobile/components/ui/Button::Button` | apps/mobile/components/ui/Button.tsx | all | component | Wrapped component. Props: className, variant, size, style, androidRootClassName, ...props. Hooks: useColorScheme. Renders: TextClassContext.Provider, Root, Pressable. |
| `apps/mobile/components/ui/ChevronRight::ChevronRight` | apps/mobile/components/ui/ChevronRight.tsx | all | component | Function component. Props: color, ...props. Hooks: useColorScheme. Renders: ChevronRightIcon. |
| `apps/mobile/components/ui/Divider::Divider` | apps/mobile/components/ui/Divider.tsx | all | component | Function component. Props: className, orientation, ...props. Renders: View. |
| `apps/mobile/components/ui/emoji-picker::EmojiCell` | apps/mobile/components/ui/emoji-picker.tsx | all | component | Wrapped component. Props: emoji, selectedEmoji, size, onSelect, chooseLabel. Renders: Pressable, Text. |
| `apps/mobile/components/ui/emoji-picker::EmojiPicker` | apps/mobile/components/ui/emoji-picker.tsx | all | component | Function component. Props: value, onChange. Hooks: useState, useRef, useWindowDimensions, useSafeAreaInsets, useColorScheme, useMemo, +3 more. Renders: EmojiCell, Pressable, Text, Modal, KeyboardAvoidingView, View. |
| `apps/mobile/components/ui/EmptyState::EmptyState` | apps/mobile/components/ui/EmptyState.tsx | all | component | Function component. Props: icon, title, subtitle, actionLabel, onAction. Hooks: useColorScheme. Renders: Animated.View, View, AppIcon, Text, Button. |
| `apps/mobile/components/ui/FAB/FAB::FAB` | apps/mobile/components/ui/FAB/FAB.tsx | all | component | Function component. Props: children. Hooks: useColorScheme. Renders: View. |
| `apps/mobile/components/ui/FAB/FAB.ios::FAB` | apps/mobile/components/ui/FAB/FAB.ios.tsx | all | component | Function component. Props: children. Hooks: useSafeAreaInsets, useColorScheme. Renders: View, GlassView. |
| `apps/mobile/components/ui/FullPageSpinner::FullPageSpinner` | apps/mobile/components/ui/FullPageSpinner.tsx | all | component | Function component. Renders: View, ActivityIndicator. |
| `apps/mobile/components/ui/GroupedList::GroupedHeader` | apps/mobile/components/ui/GroupedList.tsx | all | component | Function component. Props: label. Renders: Text. |
| `apps/mobile/components/ui/GroupedList::GroupedListRow` | apps/mobile/components/ui/GroupedList.tsx | all | component | Function component. Props: children, isFirst, isLast, separatorInset. Renders: View. |
| `apps/mobile/components/ui/GroupedList::GroupedSection` | apps/mobile/components/ui/GroupedList.tsx | all | component | Function component. Props: children, header, footer. Renders: View, GroupedHeader, Text. |
| `apps/mobile/components/ui/GroupedList::NavigationRow` | apps/mobile/components/ui/GroupedList.tsx | all | component | Function component. Props: label, value, onPress. Renders: Pressable, Text, ChevronRight. |
| `apps/mobile/components/ui/GroupedList::RowSeparator` | apps/mobile/components/ui/GroupedList.tsx | all | component | Function component. Renders: View. |
| `apps/mobile/components/ui/Input::Input` | apps/mobile/components/ui/Input.tsx | all | component | Wrapped component. Props: className, label, labelClasses, inputClasses, loading, ...props. Hooks: useColorScheme. Renders: View, Text, TextInput, ActivityIndicator. |
| `apps/mobile/components/ui/SearchInput/SearchInput::SearchInput` | apps/mobile/components/ui/SearchInput/SearchInput.tsx | all | component | Wrapped component. Props: value, onChangeText, placeholder, containerClassName, iconContainerClassName, className, +2 more. Hooks: useColorScheme, useTranslation, useAugmentedRef, useControllableState. Renders: Button, View, TailwindResolver, SearchIcon, TextInput, Animated.View. |
| `apps/mobile/components/ui/SearchInput/SearchInput.ios::SearchInput` | apps/mobile/components/ui/SearchInput/SearchInput.ios.tsx | all | component | Wrapped component. Props: value, onChangeText, onFocus, placeholder, cancelText, containerClassName, +5 more. Hooks: useAugmentedRef, useTranslation, useSharedTranslation, useState, useSharedValue, useEffect, +2 more. Renders: Animated.View, View, TailwindResolver, SearchIcon, TextInput, Pressable. |
| `apps/mobile/components/ui/SegmentedControl::SegmentedControl` | apps/mobile/components/ui/SegmentedControl.tsx | all | component | Function component. Props: options, value, onChange. Renders: View, Pressable, Text. |
| `apps/mobile/components/ui/SheetHeader::HeaderTextButton` | apps/mobile/components/ui/SheetHeader.tsx | all | component | Function component. Props: label, onPress, emphasized, disabled. Renders: Pressable, Text. |
| `apps/mobile/components/ui/SheetHeader::SheetHeader` | apps/mobile/components/ui/SheetHeader.tsx | all | component | Function component. Props: title, onCancel, onSave, saveLabel, saveDisabled, isSaving. Hooks: useCommonActions. Renders: Stack.Screen, HeaderTextButton, ActivityIndicator. |
| `apps/mobile/components/ui/Skeleton::Skeleton` | apps/mobile/components/ui/Skeleton.tsx | all | component | Function component. Props: className, ...props. Hooks: useRef, useEffect. Renders: Animated.View. |
| `apps/mobile/components/ui/Text::Text` | apps/mobile/components/ui/Text.tsx | all | component | Function component. Props: className, variant, color, ...props. Hooks: useContext. Renders: RNText. |
| `apps/mobile/components/ui/Toast::ActionToast` | apps/mobile/components/ui/Toast.tsx | all | component | Function component. Props: message, actionLabel, onAction. Renders: View, Text, Pressable. |
| `apps/mobile/lib/client-config::ClientConfigProvider` | apps/mobile/lib/client-config.tsx | all | component | Function component. Props: children. Hooks: useTRPC, useQuery. Renders: SharedClientConfigProvider. |
| `apps/mobile/lib/i18n/provider::I18nProvider` | apps/mobile/lib/i18n/provider.tsx | all | component | Function component. Props: children. Hooks: useAppSettings, useEffect. Renders: I18nextProvider. |
| `apps/mobile/lib/providers::Providers` | apps/mobile/lib/providers.tsx | all | component | Function component. Props: children. Hooks: useColorScheme, useAppSettings, useState, useEffect, useMemo. Renders: FullPageSpinner, PersistQueryClientProvider, TRPCSettingsProvider, ClientConfigProvider, I18nProvider, OfflineDownloadSync. |
| `apps/mobile/lib/readerSettings::ReaderSettingsProvider` | apps/mobile/lib/readerSettings.tsx | all | component | Function component. Props: children. Hooks: useCallback. Renders: BaseReaderSettingsProvider. |
| `apps/mobile/lib/useConnectionStatus::ConnectionStatusProvider` | apps/mobile/lib/useConnectionStatus.tsx | all | component | Function component. Props: children, enabled. Hooks: useConnectionStatusMonitor. Renders: ConnectionStatusContext.Provider. |
| `apps/web/app/admin/admin_tools/page::AdminToolsPage` | apps/web/app/admin/admin_tools/page.tsx | all | component | Function component. Renders: div, BookmarkDebugger. |
| `apps/web/app/admin/background_jobs/page::BackgroundJobsPage` | apps/web/app/admin/background_jobs/page.tsx | all | component | Function component. Renders: BackgroundJobs. |
| `apps/web/app/admin/layout::AdminLayout` | apps/web/app/admin/layout.tsx | all | component | Function component. Props: children. Hooks: useTranslation. Renders: div, AdminsOnly, SidebarLayout, SectionSidebar, SectionMobileBar, AdminNotices. |
| `apps/web/app/admin/overview/page::AdminOverviewPage` | apps/web/app/admin/overview/page.tsx | all | component | Function component. Renders: div, BasicStats, ServiceConnections. |
| `apps/web/app/admin/page::AdminHomepage` | apps/web/app/admin/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: SectionIndex. |
| `apps/web/app/admin/users/page::AdminUsersPage` | apps/web/app/admin/users/page.tsx | all | component | Function component. Renders: div, HydrationBoundary, Suspense, UserListSkeleton, UserList, InvitesListSkeleton, InvitesList. |
| `apps/web/app/check-email/page::CheckEmailPage` | apps/web/app/check-email/page.tsx | all | component | Function component. Hooks: useSearchParams, useRouter, useState, useMutation. Renders: div, p, Card, CardHeader, CardTitle, CardDescription, CardContent, Button. |
| `apps/web/app/dashboard/@modal/(.)preview/[bookmarkId]/page::BookmarkPreviewPage` | apps/web/app/dashboard/@modal/(.)preview/[bookmarkId]/page.tsx | all | component | Function component. Hooks: usePreviewDialog. Renders: BookmarkPreview. |
| `apps/web/app/dashboard/@modal/(.)preview/layout::BookmarkPreviewDialogLayout` | apps/web/app/dashboard/@modal/(.)preview/layout.tsx | all | component | Function component. Props: children. Hooks: useParams, useRouter, useRef, useState, usePreviewNavigation. Renders: Dialog, VisuallyHidden, DialogHeader, DialogTitle, DialogContent, PreviewDialogContext.Provider. |
| `apps/web/app/dashboard/archive/page::ArchivedBookmarkPage` | apps/web/app/dashboard/archive/page.tsx | all | component | Function component. Renders: Bookmarks. |
| `apps/web/app/dashboard/bookmarks/page::BookmarksPage` | apps/web/app/dashboard/bookmarks/page.tsx | all | component | Function component. Renders: div, Bookmarks. |
| `apps/web/app/dashboard/error::Error` | apps/web/app/dashboard/error.tsx | all | component | Function component. Renders: ErrorFallback. |
| `apps/web/app/dashboard/favourites/page::FavouritesBookmarkPage` | apps/web/app/dashboard/favourites/page.tsx | all | component | Function component. Renders: div, p, Bookmarks. |
| `apps/web/app/dashboard/feeds/[feedId]/page::FeedPage` | apps/web/app/dashboard/feeds/[feedId]/page.tsx | all | component | Function component. Renders: Bookmarks, PageHeader. |
| `apps/web/app/dashboard/highlights/page::HighlightsPage` | apps/web/app/dashboard/highlights/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: div, PageHeader, AllHighlights. |
| `apps/web/app/dashboard/layout::Dashboard` | apps/web/app/dashboard/layout.tsx | all | component | Function component. Props: children, modal. Renders: Home, Search, Tag, Highlighter, Archive, ClipboardList. |
| `apps/web/app/dashboard/lists/[listId]/page::ListPage` | apps/web/app/dashboard/lists/[listId]/page.tsx | all | component | Function component. Renders: BookmarkListContextProvider, Bookmarks, ListHeader. |
| `apps/web/app/dashboard/lists/page::ListsPage` | apps/web/app/dashboard/lists/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: div, PageHeader, NewListButton, PendingInvitationsCard, AllListsView. |
| `apps/web/app/dashboard/not-found::NotFound` | apps/web/app/dashboard/not-found.tsx | all | component | Function component. Hooks: useTranslation. Renders: div, h1, p, FileQuestion, Button, ArrowLeft, Link, Home. |
| `apps/web/app/dashboard/preview/[bookmarkId]/page::BookmarkPreviewPage` | apps/web/app/dashboard/preview/[bookmarkId]/page.tsx | all | component | Function component. Renders: div, BookmarkPreview. |
| `apps/web/app/dashboard/search/page::SearchComp` | apps/web/app/dashboard/search/page.tsx | all | component | Function component. Hooks: useBookmarkSearch, useInSearchPageStore, useSortOrderStore, useEffect. Renders: div, BookmarksGrid, BookmarksGridSkeleton. |
| `apps/web/app/dashboard/search/page::SearchPage` | apps/web/app/dashboard/search/page.tsx | all | component | Function component. Renders: Suspense, SearchComp. |
| `apps/web/app/dashboard/tags/[tagId]/page::TagPage` | apps/web/app/dashboard/tags/[tagId]/page.tsx | all | component | Function component. Renders: Bookmarks, TagHeader. |
| `apps/web/app/dashboard/tags/page::TagsPage` | apps/web/app/dashboard/tags/page.tsx | all | component | Function component. Renders: AllTagsView. |
| `apps/web/app/forgot-password/page::ForgotPasswordPage` | apps/web/app/forgot-password/page.tsx | all | component | Function component. Renders: div, KarakeepLogo, ForgotPasswordForm. |
| `apps/web/app/invite/[token]/page::InvitePage` | apps/web/app/invite/[token]/page.tsx | all | component | Function component. Props: params. Renders: div, KarakeepLogo, InviteAcceptForm. |
| `apps/web/app/layout::RootLayout` | apps/web/app/layout.tsx | all | component | Function component. Props: children. Renders: html, body, NuqsAdapter, Providers, ReactQueryDevtools, Toaster. |
| `apps/web/app/logout/page::Logout` | apps/web/app/logout/page.tsx | all | component | Function component. Hooks: useRouter, useSearchHistory, useEffect. Renders: span. |
| `apps/web/app/not-found::RootNotFound` | apps/web/app/not-found.tsx | all | component | Function component. Renders: div, NotFound. |
| `apps/web/app/public/layout::PublicLayout` | apps/web/app/public/layout.tsx | all | component | Function component. Props: children. Renders: div, main. |
| `apps/web/app/public/lists/[listId]/not-found::PublicListPageNotFound` | apps/web/app/public/lists/[listId]/not-found.tsx | all | component | Function component. Hooks: useTranslation. Renders: div, Link, KarakeepLogo, Empty, EmptyHeader, EmptyMedia, X. |
| `apps/web/app/public/lists/[listId]/page::PublicListPage` | apps/web/app/public/lists/[listId]/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: div, PublicListHeader, PublicBookmarkGrid, Empty, EmptyHeader, EmptyMedia, Bookmark. |
| `apps/web/app/reader/[bookmarkId]/page::ReaderViewPage` | apps/web/app/reader/[bookmarkId]/page.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useParams, useQuery, useReadingMinutes, useTitleScrolledAway, +7 more. Renders: div, header, span, button, main, article, BookmarkLoadError, IconTooltip, +4 more. |
| `apps/web/app/reader/layout::ReaderLayout` | apps/web/app/reader/layout.tsx | all | component | Function component. Props: children. Renders: UserSettingsContextProvider, ReaderSettingsProvider. |
| `apps/web/app/reset-password/page::ResetPasswordPage` | apps/web/app/reset-password/page.tsx | all | component | Function component. Props: searchParams. Renders: div, KarakeepLogo, ResetPasswordForm. |
| `apps/web/app/settings/ai/page::AISettingsPage` | apps/web/app/settings/ai/page.tsx | all | component | Function component. Renders: AISettings. |
| `apps/web/app/settings/api-keys/page::ApiKeysPage` | apps/web/app/settings/api-keys/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: SettingsPage, AddApiKey, ApiKeySettings. |
| `apps/web/app/settings/assets/layout::AssetsLayout` | apps/web/app/settings/assets/layout.tsx | all | component | Function component. Props: children. |
| `apps/web/app/settings/assets/page::AssetRow` | apps/web/app/settings/assets/page.tsx | all | component | Function component. Props: asset, isDetaching, onDetach. Hooks: useTranslation, useState. Renders: li, div, p, span, AssetThumbnail, Link, ActionConfirmingDialog, ActionButton, +2 more. |
| `apps/web/app/settings/assets/page::AssetsSettingsPage` | apps/web/app/settings/assets/page.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useState, useDetachBookmarkAsset, useInfiniteQuery. Renders: ul, div, FullPageSpinner, SettingsPage, Select, SelectTrigger, SelectValue, SelectContent. |
| `apps/web/app/settings/assets/page::AssetThumbnail` | apps/web/app/settings/assets/page.tsx | all | component | Function component. Props: asset. Hooks: useState. Renders: span, img. |
| `apps/web/app/settings/backups/page::BackupsPage` | apps/web/app/settings/backups/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: SettingsPage, BackupSettings. |
| `apps/web/app/settings/broken-links/layout::BrokenLinksLayout` | apps/web/app/settings/broken-links/layout.tsx | all | component | Function component. Props: children. |
| `apps/web/app/settings/broken-links/page::BrokenLinksPage` | apps/web/app/settings/broken-links/page.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQueryClient, useState, useQuery, useMutation, +1 more. Renders: div, p, span, a, SettingsPage, Empty, EmptyHeader, EmptyMedia, +2 more. |
| `apps/web/app/settings/broken-links/page::IssueBadge` | apps/web/app/settings/broken-links/page.tsx | all | component | Function component. Props: statusCode. Hooks: useTranslation. Renders: span. |
| `apps/web/app/settings/cleanups/page::CleanupsPage` | apps/web/app/settings/cleanups/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: SettingsPage, SettingsSection, TagDuplicationDetection. |
| `apps/web/app/settings/feeds/page::FeedSettingsPage` | apps/web/app/settings/feeds/page.tsx | all | component | Function component. Renders: FeedSettings. |
| `apps/web/app/settings/import/[sessionId]/page::ImportSessionDetailPage` | apps/web/app/settings/import/[sessionId]/page.tsx | all | component | Function component. Props: params. Renders: ImportSessionDetail. |
| `apps/web/app/settings/import/page::ImportSettingsPage` | apps/web/app/settings/import/page.tsx | all | component | Function component. Renders: ImportExport. |
| `apps/web/app/settings/info/page::InfoPage` | apps/web/app/settings/info/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: SettingsPage, UserDetails, ChangePassword, DeleteAccount. |
| `apps/web/app/settings/layout::SettingsLayout` | apps/web/app/settings/layout.tsx | all | component | Function component. Props: children. Hooks: useTranslation. Renders: UserSettingsContextProvider, ReaderSettingsProvider, SidebarLayout, SectionSidebar, SectionMobileBar. |
| `apps/web/app/settings/page::SettingsHomepage` | apps/web/app/settings/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: SectionIndex. |
| `apps/web/app/settings/preferences/page::PreferencesPage` | apps/web/app/settings/preferences/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: SettingsPage, UserOptions. |
| `apps/web/app/settings/reading/page::ReadingPage` | apps/web/app/settings/reading/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: SettingsPage, ReadingSettings. |
| `apps/web/app/settings/rules/layout::RulesLayout` | apps/web/app/settings/rules/layout.tsx | all | component | Function component. Props: children. |
| `apps/web/app/settings/rules/page::RulesSettingsPage` | apps/web/app/settings/rules/page.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useState, useQuery. Renders: div, SettingsPage, Button, PlusCircle, SettingsSection, FullPageSpinner, RuleList. |
| `apps/web/app/settings/stats/layout::StatsLayout` | apps/web/app/settings/stats/layout.tsx | all | component | Function component. Props: children. |
| `apps/web/app/settings/stats/page::BarRow` | apps/web/app/settings/stats/page.tsx | all | component | Function component. Props: label, value, maxValue, icon, rank. Renders: div, span. |
| `apps/web/app/settings/stats/page::BookmarksAddedStat` | apps/web/app/settings/stats/page.tsx | all | component | Function component. Props: counts. Hooks: useTranslation, useState. Renders: StatTile, RadioGroupPrimitive.Root, RadioGroupPrimitive.Item. |
| `apps/web/app/settings/stats/page::ColumnChart` | apps/web/app/settings/stats/page.tsx | all | component | Function component. Props: title, data, labels, axisLabels, summary. Hooks: useTranslation, useWidth. Renders: div, h4, p, span, button, Tooltip, TooltipTrigger, TooltipPortal, +1 more. |
| `apps/web/app/settings/stats/page::StatsPage` | apps/web/app/settings/stats/page.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQuery. Renders: div, span, p, SettingsPage, StatTile, Empty, EmptyHeader, EmptyMedia, +1 more. |
| `apps/web/app/settings/subscription/page::SubscriptionPage` | apps/web/app/settings/subscription/page.tsx | all | component | Function component. Hooks: useTranslation. Renders: SettingsPage, SubscriptionSettings, QuotaProgress. |
| `apps/web/app/settings/webhooks/page::WebhookSettingsPage` | apps/web/app/settings/webhooks/page.tsx | all | component | Function component. Renders: WebhookSettings. |
| `apps/web/app/signin/page::SignInPage` | apps/web/app/signin/page.tsx | all | component | Function component. Props: searchParams. Renders: div, KarakeepLogo, SignInForm. |
| `apps/web/app/signup/page::SignUpPage` | apps/web/app/signup/page.tsx | all | component | Function component. Props: searchParams. Renders: div, KarakeepLogo, SignUpForm. |
| `apps/web/app/verify-email/page::VerifyEmailPage` | apps/web/app/verify-email/page.tsx | all | component | Function component. Hooks: useSearchParams, useRouter, useState, useMutation, useEffect. Renders: div, Card, CardHeader, CardTitle, CardDescription, CardContent, Loader2. |
| `apps/web/components/admin/AddUserDialog::AddUserDialog` | apps/web/components/admin/AddUserDialog.tsx | all | component | Function component. Props: children. Hooks: useTRPC, useTranslation, useQueryClient, useState, useForm, useMutation, +1 more. Renders: form, div, Dialog, DialogTrigger, DialogContent, DialogHeader, DialogTitle, Form. |
| `apps/web/components/admin/AdminCard::AdminCard` | apps/web/components/admin/AdminCard.tsx | all | component | Function component. Props: className, children. Renders: div. |
| `apps/web/components/admin/AdminNotices::AdminNoticeBadge` | apps/web/components/admin/AdminNotices.tsx | all | component | Function component. Hooks: useAdminNotices. Renders: Badge. |
| `apps/web/components/admin/AdminNotices::AdminNotices` | apps/web/components/admin/AdminNotices.tsx | all | component | Function component. Hooks: useAdminNotices. Renders: div, AdminCard, Alert, AlertCircle, AlertTitle, AlertDescription. |
| `apps/web/components/admin/AdminsOnly::AdminsOnly` | apps/web/components/admin/AdminsOnly.tsx | all | component | Function component. Hooks: useTranslation. Renders: main, Empty, EmptyHeader, EmptyMedia, ShieldAlert, EmptyTitle, EmptyDescription. |
| `apps/web/components/admin/BackgroundJobs::BackgroundJobs` | apps/web/components/admin/BackgroundJobs.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQuery, useJobActions. Renders: div, h2, p, Skeleton, JobCardSkeleton, AdminCard, JobStatusExplanation, JobCard. |
| `apps/web/components/admin/BackgroundJobs::JobCard` | apps/web/components/admin/BackgroundJobs.tsx | all | component | Function component. Props: title, icon, stats, description, actions. Hooks: useTranslation. Renders: div, span, h4, Card, CardHeader, Icon, CardTitle, Badge, +1 more. |
| `apps/web/components/admin/BackgroundJobs::JobCardSkeleton` | apps/web/components/admin/BackgroundJobs.tsx | all | component | Function component. Renders: div, Card, CardHeader, Skeleton, CardContent. |
| `apps/web/components/admin/BackgroundJobs::JobStatusExplanation` | apps/web/components/admin/BackgroundJobs.tsx | all | component | Function component. Hooks: useTranslation. Renders: div, h4, p, Card, CardHeader, CardTitle, HelpCircle, CardContent, +1 more. |
| `apps/web/components/admin/BasicStats::BasicStats` | apps/web/components/admin/BasicStats.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQuery. Renders: div, StatsSkeleton, AdminCard, ReleaseInfo. |
| `apps/web/components/admin/BasicStats::ReleaseInfo` | apps/web/components/admin/BasicStats.tsx | all | component | Function component. Hooks: useClientConfig, useLatestRelease. Renders: a, div, span. |
| `apps/web/components/admin/BasicStats::StatsSkeleton` | apps/web/components/admin/BasicStats.tsx | all | component | Function component. Renders: div, AdminCard. |
| `apps/web/components/admin/BookmarkDebugger::BookmarkDebugger` | apps/web/components/admin/BookmarkDebugger.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useState, useQueryState, useEffect, useQuery, +1 more. Renders: div, h2, h3, p, span, button, Badge, Icon, +4 more. |
| `apps/web/components/admin/CreateInviteDialog::CreateInviteDialog` | apps/web/components/admin/CreateInviteDialog.tsx | all | component | Function component. Props: children. Hooks: useTranslation, useTRPC, useQueryClient, useState, useForm, useMutation. Renders: form, p, div, Dialog, DialogTrigger, DialogContent, DialogHeader, DialogTitle, +1 more. |
| `apps/web/components/admin/InvitesList::InvitesList` | apps/web/components/admin/InvitesList.tsx | all | component | Function component. Hooks: useTranslation, useTRPC, useQueryClient, useSuspenseQuery, useMutation. Renders: div, p, span, Table, TableHeader, TableHead, TableBody, TableRow, +1 more. |
| `apps/web/components/admin/InvitesListSkeleton::InvitesListSkeleton` | apps/web/components/admin/InvitesListSkeleton.tsx | all | component | Function component. Renders: div, AdminCard, Skeleton, Table, TableHeader, TableRow, TableHead. |
| `apps/web/components/admin/ResetPasswordDialog::ResetPasswordDialog` | apps/web/components/admin/ResetPasswordDialog.tsx | all | component | Function component. Props: userId, open, setOpen, onCloseAutoFocus. Hooks: useTranslation, useTRPC, useForm, useMutation, useEffect. Renders: form, div, Dialog, DialogContent, DialogHeader, DialogTitle, Form, FormField. |
| `apps/web/components/admin/ServiceConnections::ConnectionsSkeleton` | apps/web/components/admin/ServiceConnections.tsx | all | component | Function component. Renders: div, AdminCard. |
| `apps/web/components/admin/ServiceConnections::ConnectionStatus` | apps/web/components/admin/ServiceConnections.tsx | all | component | Function component. Props: label, configured, connected, pluginName, error. Hooks: useTranslation. Renders: div, span, p. |
| `apps/web/components/admin/ServiceConnections::ServiceConnections` | apps/web/components/admin/ServiceConnections.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQuery. Renders: div, p, ConnectionsSkeleton, AdminCard, ConnectionStatus. |
| `apps/web/components/admin/UpdateUserDialog::UpdateUserDialog` | apps/web/components/admin/UpdateUserDialog.tsx | all | component | Function component. Props: userId, currentRole, currentQuota, currentStorageQuota, open, setOpen, +1 more. Hooks: useTranslation, useTRPC, useQueryClient, useForm, useMutation, useEffect. Renders: form, div, input, Dialog, DialogContent, DialogHeader, DialogTitle, Form, +1 more. |
| `apps/web/components/admin/UserList::UserRow` | apps/web/components/admin/UserList.tsx | all | component | Wrapped component. Props: user, stats, isSelf, t, openDialog. Renders: TableRow, TableCell, ButtonWithTooltip, Trash, KeyRound, Pencil. |
| `apps/web/components/admin/UserList::UsersSection` | apps/web/components/admin/UserList.tsx | all | component | Function component. Hooks: useTRPC, useQueryClient, useTranslation, useSession, useSuspenseQuery, useState, +3 more. Renders: div, span, AdminCard, AddUserDialog, ButtonWithTooltip, UserPlus, Table, TableHeader. |
| `apps/web/components/admin/UserListSkeleton::UserListSkeleton` | apps/web/components/admin/UserListSkeleton.tsx | all | component | Function component. Renders: div, AdminCard, Skeleton, Table, TableHeader, TableRow, TableHead. |
| `apps/web/components/dashboard/bookmarks/AssetCard::AssetCard` | apps/web/components/dashboard/bookmarks/AssetCard.tsx | all | component | Function component. Props: bookmark, className, bookmarkIndex. Hooks: useTranslation. Renders: div, BookmarkLayoutAdaptingCard, Link, FooterLinkURL, AssetImage. |
| `apps/web/components/dashboard/bookmarks/AssetCard::AssetImage` | apps/web/components/dashboard/bookmarks/AssetCard.tsx | all | component | Function component. Props: bookmark, className. Hooks: useBookmarkDisplaySettings, useState. Renders: span, Link, CardImage, FileText, Image. |
| `apps/web/components/dashboard/bookmarks/BookmarkActionBar::BookmarkActionBar` | apps/web/components/dashboard/bookmarks/BookmarkActionBar.tsx | all | component | Function component. Props: bookmark, compact, hideFavourite. Hooks: useTranslation, useUserSettings, useBulkActionsStore. Renders: div, span, FavouritedActionIcon, FavouriteButton, Tooltip, TooltipTrigger, Link, Maximize2. |
| `apps/web/components/dashboard/bookmarks/BookmarkActionBar::FavouriteButton` | apps/web/components/dashboard/bookmarks/BookmarkActionBar.tsx | all | component | Function component. Props: bookmark, className. Hooks: useTranslation, useSession, useClientConfig, useBulkActionsStore, useUpdateBookmark. Renders: span, FavouritedActionIcon, ButtonWithTooltip. |
| `apps/web/components/dashboard/bookmarks/BookmarkCard::BookmarkCard` | apps/web/components/dashboard/bookmarks/BookmarkCard.tsx | all | component | Function component. Props: bookmark, className, bookmarkIndex. Hooks: useTRPC, useQuery. Renders: LinkCard, TextCard, AssetCard, UnknownCard. |
| `apps/web/components/dashboard/bookmarks/BookmarkedTextEditor::BookmarkedTextEditor` | apps/web/components/dashboard/bookmarks/BookmarkedTextEditor.tsx | all | component | Function component. Props: bookmark, open, setOpen. Hooks: useTranslation, useState, useRef, useId, useUpdateBookmark. Renders: div, Dialog, DialogContent, DialogHeader, DialogTitle, Label, Input. |
| `apps/web/components/dashboard/bookmarks/BookmarkFavicon::BookmarkFavicon` | apps/web/components/dashboard/bookmarks/BookmarkFavicon.tsx | all | component | Function component. Props: src, domain, className. Hooks: useState. Renders: span, Globe, Image. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::BookmarkLayoutAdaptingCard` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: props: Props. Hooks: useBookmarkLayout. Renders: GridView, ListView, CompactView. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::BottomRow` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: footer, tags, toolbar, hideFavourite, bookmark. Renders: div, span, BookmarkFormattedCreatedAt, BookmarkActionBar. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::BulkEditSelectionOverlay` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: bookmark. Hooks: useBulkActionsStore, useSession, useTranslation. Renders: button. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::CardHoverActions` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: bookmark, className. Hooks: useTranslation, useBulkActionsStore, useSession, useClientConfig, useArchiveBookmarkWithUndo. Renders: DragHandle, ButtonWithTooltip, Square, ArchivedActionIcon. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::CardToolbar` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: bookmark, inline, starOnly. Hooks: useBulkActionsStore, useSession. Renders: div, span, FavouriteButton, SelectionCheckbox, CardHoverActions. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::CompactRowActions` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: bookmark. Hooks: useBulkActionsStore. Renders: div, CardHoverActions. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::CompactView` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: bookmark, title, footer, className, bookmarkIndex. Hooks: useTranslation, useBookmarkDisplaySettings, useBulkActionsStore. Renders: div, span, BulkEditSelectionOverlay, OwnerIndicator, KeyboardPreviewLink, BookmarkFavicon, NotebookPen, ImageIcon. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::DragHandle` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: bookmark, className. Hooks: useTranslation, useCallback. Renders: div, Tooltip, TooltipTrigger, GripVertical, TooltipPortal, TooltipContent. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::GridView` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: bookmark, image, imageIsPlaceholder, title, content, footer, +4 more. Hooks: useBookmarkDisplaySettings. Renders: div, BulkEditSelectionOverlay, OwnerIndicator, KeyboardPreviewLink, CardToolbar, NoteTypeRow, NotePreview. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::KeyboardPreviewLink` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: bookmark. Hooks: useTranslation. Renders: Link. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::ListView` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: bookmark, image, title, content, footer, className, +1 more. Hooks: useBookmarkDisplaySettings. Renders: div, p, BulkEditSelectionOverlay, OwnerIndicator, KeyboardPreviewLink, NotePreview, TagList, BottomRow. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::NoteTypeRow` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Hooks: useTranslation. Renders: div, span, NotebookPen. |
| `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::OwnerIndicator` | apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx | all | component | Function component. Props: bookmark, className. Hooks: useTRPC, useBookmarkListContext, useQuery. Renders: div, BookmarkOwnerIcon. |
| `apps/web/components/dashboard/bookmarks/BookmarkMarkdownComponent::BookmarkMarkdownComponent` | apps/web/components/dashboard/bookmarks/BookmarkMarkdownComponent.tsx | all | component | Function component. Props: children, readOnly, className. Hooks: useTranslation, useUpdateBookmark. Renders: div, MarkdownReadonly, MarkdownEditor. |
| `apps/web/components/dashboard/bookmarks/BookmarkOptions::BookmarkOptions` | apps/web/components/dashboard/bookmarks/BookmarkOptions.tsx | all | component | Function component. Props: bookmark, hiddenActions, showPreviewAction, trigger, triggerTooltip. Hooks: useTranslation, useRouter, useMediaQuery, useSession, useClientConfig, useBulkActionsStore, +16 more. Renders: span, input, RotateCw, Maximize2, Square, Pencil, Tag, SquarePen. |
| `apps/web/components/dashboard/bookmarks/BookmarkOptions::BookmarkOptionsSheet` | apps/web/components/dashboard/bookmarks/BookmarkOptions.tsx | all | component | Function component. Props: bookmark, groups, onCloseAutoFocus, trigger. Hooks: useTranslation, useState. Renders: div, h3, Dialog, DialogTrigger, DialogContent, DialogTitle, DialogDescription, Fragment. |
| `apps/web/components/dashboard/bookmarks/BookmarkOptions::SheetAction` | apps/web/components/dashboard/bookmarks/BookmarkOptions.tsx | all | component | Function component. Props: item, onSelect. Renders: button, span. |
| `apps/web/components/dashboard/bookmarks/BookmarkOwnerIcon::BookmarkOwnerIcon` | apps/web/components/dashboard/bookmarks/BookmarkOwnerIcon.tsx | all | component | Function component. Props: ownerName, ownerAvatar. Renders: p, Tooltip, TooltipTrigger, UserAvatar, TooltipContent. |
| `apps/web/components/dashboard/bookmarks/Bookmarks::Bookmarks` | apps/web/components/dashboard/bookmarks/Bookmarks.tsx | all | component | Function component. Props: query, header, showDivider, showEditorCard. Renders: div, Separator, UpdatableBookmarksGrid. |
| `apps/web/components/dashboard/bookmarks/BookmarksGrid::BookmarkGridItem` | apps/web/components/dashboard/bookmarks/BookmarksGrid.tsx | all | component | Wrapped component. Props: bookmark, index. Hooks: useKeyboardNavigationStore. Renders: ErrorBoundary, UnknownCard, StyledBookmarkCard, BookmarkCard. |
| `apps/web/components/dashboard/bookmarks/BookmarksGrid::BookmarksGrid` | apps/web/components/dashboard/bookmarks/BookmarksGrid.tsx | all | component | Function component. Props: bookmarks, hasNextPage, fetchNextPage, isFetchingNextPage, showEditorCard, isSearch. Hooks: useTranslation, useBookmarkLayout, useGridColumns, useActiveGridColumns, useBulkActionsStore, useInBookmarkGridStore, +5 more. Renders: div, NoBookmarksBanner, KeyboardShortcutsDialog, StyledBookmarkCard, EditorCard, BookmarkGridItem, Masonry. |
| `apps/web/components/dashboard/bookmarks/BookmarksGrid::StyledBookmarkCard` | apps/web/components/dashboard/bookmarks/BookmarksGrid.tsx | all | component | Function component. Props: children, className, ...props. Renders: Slot. |
| `apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton::BookmarksGridSkeleton` | apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton.tsx | all | component | Function component. Props: count. Hooks: useBookmarkLayout, useGridColumns, useMemo. Renders: div, Masonry, GridCardSkeleton, ListRowSkeleton, CompactRowSkeleton. |
| `apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton::CompactRowSkeleton` | apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton.tsx | all | component | Function component. Renders: div, Skeleton. |
| `apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton::GridCardSkeleton` | apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton.tsx | all | component | Function component. Props: imageHeight. Renders: div, Skeleton. |
| `apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton::ListRowSkeleton` | apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton.tsx | all | component | Function component. Renders: div, Skeleton. |
| `apps/web/components/dashboard/bookmarks/BookmarkTagsEditor::BookmarkTagsEditor` | apps/web/components/dashboard/bookmarks/BookmarkTagsEditor.tsx | all | component | Function component. Props: bookmark, disabled, placeholder, variant. Hooks: useTranslation, useUpdateBookmarkTags. Renders: div, TagsEditor. |
| `apps/web/components/dashboard/bookmarks/BulkManageListsModal::BulkManageListsModal` | apps/web/components/dashboard/bookmarks/BulkManageListsModal.tsx | all | component | Function component. Props: bookmarkIds, open, setOpen. Hooks: useTranslation, useForm, useAddBookmarkToList. Renders: form, Dialog, DialogContent, Form, DialogHeader, DialogTitle, FormField. |
| `apps/web/components/dashboard/bookmarks/BulkTagModal::BulkTagModal` | apps/web/components/dashboard/bookmarks/BulkTagModal.tsx | all | component | Function component. Props: bookmarkIds, open, setOpen. Hooks: useTranslation, useTRPC, useFocusTagInputOnOpen, useQueries, useUpdateBookmarkTags. Renders: h3, div, p, ul, Dialog, DialogContent, DialogHeader, DialogTitle, +2 more. |
| `apps/web/components/dashboard/bookmarks/BulkTagModal::TagRow` | apps/web/components/dashboard/bookmarks/BulkTagModal.tsx | all | component | Function component. Props: name, count, total, onAddToAll, onRemove. Hooks: useTranslation, useState. Renders: li, span, div, ActionButtonWithTooltip, LoadingSpinner, Plus, X. |
| `apps/web/components/dashboard/bookmarks/CardImage::CardImage` | apps/web/components/dashboard/bookmarks/CardImage.tsx | all | component | Function component. Props: src, alt, className, isScreenshot. Hooks: useState. Renders: Image. |
| `apps/web/components/dashboard/bookmarks/DeleteBookmarkConfirmationDialog::BulkDeleteDescription` | apps/web/components/dashboard/bookmarks/DeleteBookmarkConfirmationDialog.tsx | all | component | Function component. Props: bookmarks. Hooks: useTranslation. Renders: div, p, ul, li. |
| `apps/web/components/dashboard/bookmarks/DeleteBookmarkConfirmationDialog::DeleteBookmarkConfirmationDialog` | apps/web/components/dashboard/bookmarks/DeleteBookmarkConfirmationDialog.tsx | all | component | Function component. Props: bookmark, children, open, setOpen. Hooks: useTranslation, usePathname, useRouter, useDeleteBookmark. Renders: p, ActionConfirmingDialog, ActionButton. |
| `apps/web/components/dashboard/bookmarks/EditBookmarkDialog::EditBookmarkDialog` | apps/web/components/dashboard/bookmarks/EditBookmarkDialog.tsx | all | component | Function component. Props: open, setOpen, bookmark, children. Hooks: useTRPC, useTranslation, useQuery, useForm, useUpdateBookmark, useDialogFormReset, +1 more. Renders: form, div, span, Dialog, DialogTrigger, DialogContent, DialogHeader, DialogTitle, +1 more. |
| `apps/web/components/dashboard/bookmarks/EditorCard::EditorCard` | apps/web/components/dashboard/bookmarks/EditorCard.tsx | all | component | Function component. Props: className. Hooks: useTranslation, useRef, useState, useClientConfig, useBookmarkLayout, useForm, +5 more. Renders: form, div, p, BookmarkSavedToast, Form, Kbd, Separator, FormItem, +1 more. |
| `apps/web/components/dashboard/bookmarks/FooterLinkURL::FooterLinkURL` | apps/web/components/dashboard/bookmarks/FooterLinkURL.tsx | all | component | Function component. Props: url. Hooks: useTranslation. Renders: span, Tooltip, TooltipTrigger, Link, ExternalLink, TooltipPortal, TooltipContent. |
| `apps/web/components/dashboard/bookmarks/icons::ArchivedActionIcon` | apps/web/components/dashboard/bookmarks/icons.tsx | all | component | Function component. Props: archived, className, size, strokeWidth. Renders: ArchiveRestore, Archive. |
| `apps/web/components/dashboard/bookmarks/icons::FavouritedActionIcon` | apps/web/components/dashboard/bookmarks/icons.tsx | all | component | Function component. Props: favourited, className, size, strokeWidth. Renders: Star. |
| `apps/web/components/dashboard/bookmarks/icons::SelectionCheckbox` | apps/web/components/dashboard/bookmarks/icons.tsx | all | component | Function component. Props: checked. Renders: span, Check. |
| `apps/web/components/dashboard/bookmarks/LinkCard::CrawlFailedIcon` | apps/web/components/dashboard/bookmarks/LinkCard.tsx | all | component | Function component. Hooks: useTranslation. Renders: span, Tooltip, TooltipTrigger, TriangleAlert, TooltipPortal, TooltipContent. |
| `apps/web/components/dashboard/bookmarks/LinkCard::LinkCard` | apps/web/components/dashboard/bookmarks/LinkCard.tsx | all | component | Function component. Props: bookmark, className, bookmarkIndex. Renders: span, BookmarkLayoutAdaptingCard, LinkTitle, CrawlFailedIcon, FooterLinkURL, LinkImage. |
| `apps/web/components/dashboard/bookmarks/LinkCard::LinkImage` | apps/web/components/dashboard/bookmarks/LinkCard.tsx | all | component | Function component. Props: bookmark, className. Hooks: useOnClickUrl, useBookmarkDisplaySettings. Renders: div, Link, BookmarkFavicon, Image, CardImage. |
| `apps/web/components/dashboard/bookmarks/LinkCard::LinkTitle` | apps/web/components/dashboard/bookmarks/LinkCard.tsx | all | component | Function component. Props: bookmark. Hooks: useOnClickUrl. Renders: Link. |
| `apps/web/components/dashboard/bookmarks/ManageListsModal::ManageListsModal` | apps/web/components/dashboard/bookmarks/ManageListsModal.tsx | all | component | Function component. Props: bookmarkId, open, setOpen. Hooks: useTRPC, useTranslation, useQueryClient, useClientConfig, useMediaQuery, useBookmarkLists, +4 more. Renders: div, span, Dialog, DialogContent, DialogHeader, DialogTitle, LoadingSpinner, Command. |
| `apps/web/components/dashboard/bookmarks/NoBookmarksBanner::NoBookmarksBanner` | apps/web/components/dashboard/bookmarks/NoBookmarksBanner.tsx | all | component | Function component. Props: isSearch. Hooks: useTranslation. Renders: div, h3, p, Icon. |
| `apps/web/components/dashboard/bookmarks/NotePreview::NotePreview` | apps/web/components/dashboard/bookmarks/NotePreview.tsx | all | component | Function component. Props: note, bookmarkId, className. Hooks: useTranslation, useState. Renders: button, span, div, Popover, PopoverTrigger, NotepadText, PopoverContent, Link, +1 more. |
| `apps/web/components/dashboard/bookmarks/SummarizeBookmarkArea::AISummary` | apps/web/components/dashboard/bookmarks/SummarizeBookmarkArea.tsx | all | component | Function component. Props: bookmarkId, summary, readOnly. Hooks: useTranslation, useState, useSummarizeBookmark, useUpdateBookmark. Renders: div, span, SidebarSectionHeading, MarkdownReadonly, IconTooltip, ActionButton, LoadingSpinner, RefreshCw. |
| `apps/web/components/dashboard/bookmarks/SummarizeBookmarkArea::SummarizeBookmarkArea` | apps/web/components/dashboard/bookmarks/SummarizeBookmarkArea.tsx | all | component | Function component. Props: bookmark, readOnly. Hooks: useTranslation, useSummarizeBookmark, useClientConfig. Renders: div, span, AISummary, ActionButton, Sparkles. |
| `apps/web/components/dashboard/bookmarks/TagList::TagList` | apps/web/components/dashboard/bookmarks/TagList.tsx | all | component | Function component. Props: bookmark, loading, className. Hooks: useSession. Renders: div, span, Skeleton, Link. |
| `apps/web/components/dashboard/bookmarks/TagModal::TagModal` | apps/web/components/dashboard/bookmarks/TagModal.tsx | all | component | Function component. Props: bookmark, open, setOpen. Hooks: useTRPC, useTranslation, useFocusTagInputOnOpen, useQuery. Renders: Dialog, DialogContent, DialogHeader, DialogTitle, BookmarkTagsEditor. |
| `apps/web/components/dashboard/bookmarks/TagsEditor::TagsEditor` | apps/web/components/dashboard/bookmarks/TagsEditor.tsx | all | component | Function component. Props: tags, onAttach, onDetach, disabled, allowCreation, placeholder, +2 more. Hooks: useTRPC, useTranslation, useClientConfig, useRef, useState, useCallback, +3 more. Renders: div, span, button, label, Sparkles, IconTooltip, X, CommandList, +2 more. |
| `apps/web/components/dashboard/bookmarks/TextCard::ClampedNote` | apps/web/components/dashboard/bookmarks/TextCard.tsx | all | component | Function component. Props: bookmarkId, rowMaxHeightClass, children. Hooks: useTranslation, useRouter, useRef, useState, useEffect. Renders: div, Link. |
| `apps/web/components/dashboard/bookmarks/TextCard::TextCard` | apps/web/components/dashboard/bookmarks/TextCard.tsx | all | component | Function component. Props: bookmark, className, bookmarkIndex. Hooks: useBookmarkDisplaySettings, useBookmarkLayout. Renders: div, Link, Image, BookmarkLayoutAdaptingCard, ClampedNote, BookmarkMarkdownComponent, FooterLinkURL. |
| `apps/web/components/dashboard/bookmarks/UnknownCard::UnknownCard` | apps/web/components/dashboard/bookmarks/UnknownCard.tsx | all | component | Function component. Props: bookmark, className, bookmarkIndex. Hooks: useTranslation. Renders: h3, BookmarkLayoutAdaptingCard, Link, AlertCircle. |
| `apps/web/components/dashboard/bookmarks/UpdatableBookmarksGrid::UpdatableBookmarksGrid` | apps/web/components/dashboard/bookmarks/UpdatableBookmarksGrid.tsx | all | component | Function component. Props: query, bookmarks, showEditorCard. Hooks: useTRPC, useSortOrderStore, useInfiniteQuery, useEffect. Renders: BookmarksGrid, BookmarkGridContextProvider, UploadDropzone. |
| `apps/web/components/dashboard/BulkBookmarksAction::BulkBookmarksAction` | apps/web/components/dashboard/BulkBookmarksAction.tsx | all | component | Function component. Hooks: useTranslation, useState, usePathname, useRef, useBulkActionsStore, useBookmarkBulkMutations, +1 more. Renders: p, div, Link, ListMinus, List, Hash, FavouritedActionIcon, ArchivedActionIcon. |
| `apps/web/components/dashboard/cleanups/TagDuplicationDetention::ApplyAllButton` | apps/web/components/dashboard/cleanups/TagDuplicationDetention.tsx | all | component | Function component. Props: suggestions. Hooks: useTranslation, useState, useMergeTag. Renders: ActionConfirmingDialog, ActionButton, Check, Button. |
| `apps/web/components/dashboard/cleanups/TagDuplicationDetention::SuggestionRow` | apps/web/components/dashboard/cleanups/TagDuplicationDetention.tsx | all | component | Function component. Props: suggestion, updateMergeInto, deleteSuggestion. Hooks: useTranslation, useMergeTag. Renders: div, TableRow, TableCell, Link, Button, Check, ActionButton. |
| `apps/web/components/dashboard/cleanups/TagDuplicationDetention::TagDuplicationDetection` | apps/web/components/dashboard/cleanups/TagDuplicationDetention.tsx | all | component | Function component. Hooks: useTranslation, useTRPC, useState, useQuery, useSuggestions. Renders: div, span, p, LoadingSpinner, Empty, EmptyHeader, EmptyMedia, CircleCheck, +1 more. |
| `apps/web/components/dashboard/EditableText::EditableText` | apps/web/components/dashboard/EditableText.tsx | all | component | Function component. Hooks: useState. Renders: EditMode, ViewMode. |
| `apps/web/components/dashboard/EditableText::EditMode` | apps/web/components/dashboard/EditableText.tsx | all | component | Function component. Props: onSave, editClassName, isSaving, originalText, setEditable. Hooks: useTranslation, useRef, useEffect. Renders: div, ActionButtonWithTooltip, Check, ButtonWithTooltip, X. |
| `apps/web/components/dashboard/EditableText::ViewMode` | apps/web/components/dashboard/EditableText.tsx | all | component | Function component. Props: originalText, setEditable, viewClassName, untitledClassName. Hooks: useTranslation. Renders: div, p, Tooltip, TooltipTrigger, ButtonWithTooltip, Pencil, TooltipPortal, TooltipContent. |
| `apps/web/components/dashboard/ErrorFallback::ErrorFallback` | apps/web/components/dashboard/ErrorFallback.tsx | all | component | Function component. Hooks: useTranslation, useClientConfig, useProblemReportStore. Renders: div, h1, p, AlertTriangle, Button, RefreshCw, Link, Home, +1 more. |
| `apps/web/components/dashboard/feeds/FeedSelector::FeedSelector` | apps/web/components/dashboard/feeds/FeedSelector.tsx | all | component | Function component. Props: value, onChange, placeholder, className. Hooks: useTRPC, useQuery. Renders: LoadingSpinner, Select, SelectTrigger, SelectValue, SelectContent, SelectGroup. |
| `apps/web/components/dashboard/GlobalActions::GlobalActions` | apps/web/components/dashboard/GlobalActions.tsx | all | component | Function component. Hooks: useInBookmarkGridStore. Renders: div, ViewOptions, BulkBookmarksAction, SortOrderToggle. |
| `apps/web/components/dashboard/header/Header::Header` | apps/web/components/dashboard/header/Header.tsx | all | component | Function component. Renders: header, div, Link, KarakeepLogo, SearchInput, GlobalActions, ProfileOptions. |
| `apps/web/components/dashboard/header/ProfileOptions::SidebarProfileOptions` | apps/web/components/dashboard/header/ProfileOptions.tsx | all | component | Function component. Hooks: useTranslation, useSession, useWhoAmI, useRouter, useInBookmarkGridStore, useKeyboardNavigationStore, +4 more. Renders: div, p, a, span, ReportProblemDialog, DropdownMenu, DropdownMenuTrigger, Button, +2 more. |
| `apps/web/components/dashboard/header/ProfileOptions::ThemeSelector` | apps/web/components/dashboard/header/ProfileOptions.tsx | all | component | Function component. Hooks: useTranslation, useTheme. Renders: div, SunMoon, DropdownMenuItem, Icon. |
| `apps/web/components/dashboard/highlights/AllHighlights::AllHighlights` | apps/web/components/dashboard/highlights/AllHighlights.tsx | all | component | Function component. Props: highlights. Hooks: useTRPC, useTranslation, useState, useDebounce, useInfiniteQuery, useInView, +2 more. Renders: div, button, section, Empty, EmptyHeader, EmptyMedia, Highlighter, EmptyTitle, +1 more. |
| `apps/web/components/dashboard/highlights/AllHighlights::ArticleLink` | apps/web/components/dashboard/highlights/AllHighlights.tsx | all | component | Function component. Props: bookmarkId, bookmark. Hooks: useTranslation. Renders: span, Link. |
| `apps/web/components/dashboard/highlights/AllHighlights::ColorFilter` | apps/web/components/dashboard/highlights/AllHighlights.tsx | all | component | Function component. Props: value, onChange. Hooks: useTranslation. Renders: div, span, IconTooltip, Button, Check. |
| `apps/web/components/dashboard/highlights/AllHighlights::HighlightWithTime` | apps/web/components/dashboard/highlights/AllHighlights.tsx | all | component | Function component. Props: highlight. Hooks: useTranslation, useRelativeTime. Renders: span, HighlightCard. |
| `apps/web/components/dashboard/highlights/HighlightCard::HighlightCard` | apps/web/components/dashboard/highlights/HighlightCard.tsx | all | component | Function component. Props: highlight, clickable, href, className, readOnly, meta. Hooks: useTranslation, useDeleteHighlightWithUndo. Renders: div, blockquote, span, Wrapper, IconTooltip, ActionButton, LoadingSpinner, Trash2. |
| `apps/web/components/dashboard/highlights/HighlightCard::Wrapper` | apps/web/components/dashboard/highlights/HighlightCard.tsx | all | component | Function component. Props: className, href, onClick, children. Renders: button, div, Link. |
| `apps/web/components/dashboard/KeyboardShortcutsDialog::KeyboardShortcutsDialog` | apps/web/components/dashboard/KeyboardShortcutsDialog.tsx | all | component | Function component. Props: open, setOpen. Hooks: useTranslation, useBookmarkLayout. Renders: div, Dialog, DialogContent, DialogHeader, DialogTitle, ShortcutSection. |
| `apps/web/components/dashboard/KeyboardShortcutsDialog::ShortcutRow` | apps/web/components/dashboard/KeyboardShortcutsDialog.tsx | all | component | Function component. Props: keys, description. Renders: div, span, Kbd. |
| `apps/web/components/dashboard/KeyboardShortcutsDialog::ShortcutSection` | apps/web/components/dashboard/KeyboardShortcutsDialog.tsx | all | component | Function component. Props: title, shortcuts. Renders: div, h3, ShortcutRow. |
| `apps/web/components/dashboard/lists/AllListsView::AllListsView` | apps/web/components/dashboard/lists/AllListsView.tsx | all | component | Function component. Props: initialData, favoritesCount, archivedCount. Hooks: useTranslation, useBookmarkLists, useMemo. Renders: div, ul, section, h2, Section, ListItem, Star, Archive, +2 more. |
| `apps/web/components/dashboard/lists/AllListsView::ListItem` | apps/web/components/dashboard/lists/AllListsView.tsx | all | component | Function component. Props: name, icon, path, style, list, open, +3 more. Hooks: useTranslation. Renders: li, div, span, p, CollapsibleTrigger, ButtonWithTooltip, ChevronRight, Link, +2 more. |
| `apps/web/components/dashboard/lists/AllListsView::Section` | apps/web/components/dashboard/lists/AllListsView.tsx | all | component | Function component. Props: title, children. Renders: section, h2, div. |
| `apps/web/components/dashboard/lists/BookmarkListSelector::BookmarkListMultiSelector` | apps/web/components/dashboard/lists/BookmarkListSelector.tsx | all | component | Function component. Props: placeholder, onChange, value, isPending, allPaths, className, +1 more. Hooks: useState. Renders: div, button, span, ListSelectorComponent, X. |
| `apps/web/components/dashboard/lists/BookmarkListSelector::BookmarkListSelector` | apps/web/components/dashboard/lists/BookmarkListSelector.tsx | all | component | Function component. Props: props: BookmarkListSelectorProps. Hooks: useBookmarkLists. Renders: BookmarkListMultiSelector, BookmarkListSingleSelector. |
| `apps/web/components/dashboard/lists/BookmarkListSelector::BookmarkListSingleSelector` | apps/web/components/dashboard/lists/BookmarkListSelector.tsx | all | component | Function component. Props: placeholder, className, onChange, value, isPending, allPaths, +1 more. Hooks: useState. Renders: span, ListSelectorComponent, Button, ChevronsUpDown. |
| `apps/web/components/dashboard/lists/BookmarkListSelector::ListSelectorComponent` | apps/web/components/dashboard/lists/BookmarkListSelector.tsx | all | component | Function component. Props: onSelect, children, isItemSelected, open, setOpen, isPending, +2 more. Renders: LoadingSpinner, Popover, PopoverTrigger, PopoverContent, Command, CommandInput. |
| `apps/web/components/dashboard/lists/CollapsibleBookmarkLists::CollapsibleBookmarkLists` | apps/web/components/dashboard/lists/CollapsibleBookmarkLists.tsx | all | component | Function component. Props: render, initialData, listsData, className, isOpenFunc, filter, +1 more. Hooks: useTRPC, useBookmarkLists, useQuery. Renders: div, FullPageSpinner, ListItem. |
| `apps/web/components/dashboard/lists/CollapsibleBookmarkLists::ListItem` | apps/web/components/dashboard/lists/CollapsibleBookmarkLists.tsx | all | component | Function component. Props: node, render, level, className, isOpenFunc, listStats, +1 more. Hooks: useState, useEffect. Renders: Collapsible, CollapsibleContent, ListItem. |
| `apps/web/components/dashboard/lists/DeleteListConfirmationDialog::DeleteListConfirmationDialog` | apps/web/components/dashboard/lists/DeleteListConfirmationDialog.tsx | all | component | Function component. Props: list, children, open, setOpen. Hooks: useTranslation, usePathname, useRouter, useState, useDeleteBookmarkList. Renders: div, p, ActionConfirmingDialog, Label, Switch, ActionButton. |
| `apps/web/components/dashboard/lists/EditListModal::EditListModal` | apps/web/components/dashboard/lists/EditListModal.tsx | all | component | Function component. Props: open, setOpen, list, prefill, children. Hooks: useTranslation, useRouter, useState, useForm, useFormErrors, useEffect, +5 more. Renders: form, div, p, Dialog, DialogTrigger, DialogContent, Form, DialogHeader, +1 more. |
| `apps/web/components/dashboard/lists/LeaveListConfirmationDialog::LeaveListConfirmationDialog` | apps/web/components/dashboard/lists/LeaveListConfirmationDialog.tsx | all | component | Function component. Props: list, children, open, setOpen. Hooks: useTRPC, useTranslation, usePathname, useRouter, useQueryClient, useMutation. Renders: div, p, ActionConfirmingDialog, ActionButton. |
| `apps/web/components/dashboard/lists/ListHeader::ListHeader` | apps/web/components/dashboard/lists/ListHeader.tsx | all | component | Function component. Props: initialData. Hooks: useTRPC, useTranslation, useRouter, useQuery, useMemo. Renders: div, span, h1, p, button, ListPrivacyLabel, QueryExplainerTooltip, Sparkles, +3 more. |
| `apps/web/components/dashboard/lists/ListHeaderComponents::ListCollaboratorsIcons` | apps/web/components/dashboard/lists/ListHeaderComponents.tsx | all | component | Function component. Props: list, className. Hooks: useTRPC, useQuery. Renders: div, p, Tooltip, TooltipTrigger, UserAvatar, TooltipContent. |
| `apps/web/components/dashboard/lists/ListHeaderComponents::ListItemCount` | apps/web/components/dashboard/lists/ListHeaderComponents.tsx | all | component | Function component. Props: list, className. Hooks: useTranslation, useTRPC, useQuery. Renders: div, span. |
| `apps/web/components/dashboard/lists/ListHeaderComponents::ListPrivacyLabel` | apps/web/components/dashboard/lists/ListHeaderComponents.tsx | all | component | Function component. Props: list, className. Hooks: useTranslation. Renders: span, PrivacyIcon. |
| `apps/web/components/dashboard/lists/ListNamePicker::ListNamePicker` | apps/web/components/dashboard/lists/ListNamePicker.tsx | all | component | Function component. Props: id, placeholder, selectedNames, onToggle, excludeListId. Hooks: useTranslation, useState, useBookmarkLists. Renders: button, span, Popover, PopoverTrigger, ChevronDown, PopoverContent, Command, CommandInput. |
| `apps/web/components/dashboard/lists/ListOptions::ListOptions` | apps/web/components/dashboard/lists/ListOptions.tsx | all | component | Function component. Props: list, isOpen, onOpenChange, tooltip, children. Hooks: useTranslation, useShowArchived, useState, useRef. Renders: span, Pencil, Share, Users, Plus, FolderInput, SquareCheck. |
| `apps/web/components/dashboard/lists/ManageCollaboratorsModal::ManageCollaboratorsModal` | apps/web/components/dashboard/lists/ManageCollaboratorsModal.tsx | all | component | Function component. Props: open, setOpen, list, children, readOnly. Hooks: useTRPC, useState, useTranslation, useQueryClient, useQuery, useMutation. Renders: div, p, strong, br, Dialog, DialogTrigger, DialogContent, DialogHeader, +2 more. |
| `apps/web/components/dashboard/lists/MergeListModal::MergeListModal` | apps/web/components/dashboard/lists/MergeListModal.tsx | all | component | Function component. Props: open, setOpen, list, children. Hooks: useTranslation, useState, useForm, useEffect, useMergeLists. Renders: form, div, span, label, Dialog, DialogTrigger, DialogContent, Form, +2 more. |
| `apps/web/components/dashboard/lists/NewListButton::NewListButton` | apps/web/components/dashboard/lists/NewListButton.tsx | all | component | Function component. Hooks: useTranslation. Renders: span, EditListModal, Button, Plus. |
| `apps/web/components/dashboard/lists/PendingInvitationsCard::InvitationRow` | apps/web/components/dashboard/lists/PendingInvitationsCard.tsx | all | component | Function component. Props: invitation. Hooks: useTRPC, useTranslation, useQueryClient, useMutation. Renders: div, span, Button, Loader2, X, Check. |
| `apps/web/components/dashboard/lists/PendingInvitationsCard::PendingInvitationsCard` | apps/web/components/dashboard/lists/PendingInvitationsCard.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQuery. Renders: Card, CardHeader, CardTitle, Mail, Badge, CardDescription. |
| `apps/web/components/dashboard/lists/PublicListLink::PublicListLink` | apps/web/components/dashboard/lists/PublicListLink.tsx | all | component | Function component. Props: list. Hooks: useTranslation, useClientConfig, useEditBookmarkList. Renders: div, p, Label, Switch, Input, CopyBtnV2. |
| `apps/web/components/dashboard/lists/RssLink::RssLink` | apps/web/components/dashboard/lists/RssLink.tsx | all | component | Function component. Props: listId. Hooks: useTRPC, useTranslation, useClientConfig, useQueryClient, useMutation, useQuery, +1 more. Renders: div, p, Label, Switch, Input, CopyBtnV2, Button, Loader2. |
| `apps/web/components/dashboard/lists/ShareListModal::ShareListModal` | apps/web/components/dashboard/lists/ShareListModal.tsx | all | component | Function component. Props: open, setOpen, list, children. Hooks: useTranslation, useState. Renders: div, Dialog, DialogTrigger, DialogContent, DialogHeader, DialogTitle, DialogDescription. |
| `apps/web/components/dashboard/lists/SmartListPreview::SmartListPreview` | apps/web/components/dashboard/lists/SmartListPreview.tsx | all | component | Function component. Props: query, invalid. Hooks: useTRPC, useTranslation, useDebounce, useQuery. Renders: p, div, ul, li. |
| `apps/web/components/dashboard/lists/SmartListQueryBuilder::SmartListQueryBuilder` | apps/web/components/dashboard/lists/SmartListQueryBuilder.tsx | all | component | Function component. Props: query, onChange, listId. Hooks: useTranslation, useBookmarkLists. Renders: fieldset, p, div, ul, li, SelectItem, Label, TagNamePicker, +3 more. |
| `apps/web/components/dashboard/preview/ActionBar::ActionBar` | apps/web/components/dashboard/preview/ActionBar.tsx | all | component | Function component. Props: bookmark, className, tooltipSide. Hooks: useTranslation, useState, useUpdateBookmark, useArchiveBookmarkWithUndo. Renders: div, Tooltip, EditBookmarkDialog, TooltipTrigger, Button, Pencil, TooltipPortal. |
| `apps/web/components/dashboard/preview/ArticleTitleBlock::ArticleTitleBlock` | apps/web/components/dashboard/preview/ArticleTitleBlock.tsx | all | component | Function component. Props: bookmark, compactOnPhone, titleRef. Hooks: useTranslation, useReaderSettings, useReadingMinutes, useLocalDay. Renders: a, header, h1, div, span, ExternalLink. |
| `apps/web/components/dashboard/preview/AssetContentSection::AssetContentSection` | apps/web/components/dashboard/preview/AssetContentSection.tsx | all | component | Function component. Props: bookmark, toolbarSlot. Renders: div, ImageContentSection, PDFContentSection. |
| `apps/web/components/dashboard/preview/AssetContentSection::ImageContentSection` | apps/web/components/dashboard/preview/AssetContentSection.tsx | all | component | Function component. Props: bookmark. Renders: div, Link, Image. |
| `apps/web/components/dashboard/preview/AssetContentSection::PDFContentSection` | apps/web/components/dashboard/preview/AssetContentSection.tsx | all | component | Function component. Props: bookmark, toolbarSlot. Hooks: useTranslation, useMemo, useState. Renders: div, embed, Image, Select, IconTooltip, SelectTrigger, SelectValue, SelectContent. |
| `apps/web/components/dashboard/preview/AttachmentBox::AttachmentBox` | apps/web/components/dashboard/preview/AttachmentBox.tsx | all | component | Function component. Props: bookmark, readOnly. Hooks: useTranslation, useRememberedOpen, useAttachBookmarkAsset, useReplaceBookmarkAsset, useDetachBookmarkAsset, useUpload. Renders: div, span, p, Collapsible, CollapsibleTrigger, IconTooltip, FilePickerButton, ImagePlus, +1 more. |
| `apps/web/components/dashboard/preview/AttachmentBox::EmptyActionSlot` | apps/web/components/dashboard/preview/AttachmentBox.tsx | all | component | Function component. Renders: span. |
| `apps/web/components/dashboard/preview/BookmarkListsField::BookmarkListsField` | apps/web/components/dashboard/preview/BookmarkListsField.tsx | all | component | Function component. Props: bookmarkId. Hooks: useTRPC, useTranslation, useQueryClient, useClientConfig, useState, useQuery, +4 more. Renders: div, span, Link, Popover, PopoverTrigger, Button, Plus, PopoverContent. |
| `apps/web/components/dashboard/preview/BookmarkLoadError::BookmarkLoadError` | apps/web/components/dashboard/preview/BookmarkLoadError.tsx | all | component | Function component. Props: error, onRetry, isRetrying, className. Hooks: useTranslation, useRouter. Renders: div, Empty, EmptyHeader, EmptyMedia, FileQuestion, AlertTriangle, EmptyTitle. |
| `apps/web/components/dashboard/preview/BookmarkPreview::ArchivedStatus` | apps/web/components/dashboard/preview/BookmarkPreview.tsx | all | component | Function component. Props: bookmarkId, readOnly. Hooks: useTranslation, useArchiveBookmarkWithUndo. Renders: Badge, IconTooltip, ActionButton. |
| `apps/web/components/dashboard/preview/BookmarkPreview::BookmarkPreview` | apps/web/components/dashboard/preview/BookmarkPreview.tsx | all | component | Function component. Props: bookmarkId, initialData, placeholderData, navigation, view, onClose. Hooks: useTRPC, useTranslation, useRouter, useState, useSession, useCallback, +2 more. Renders: div, BookmarkLoadError, FullPageSpinner, ContentLoading, LinkContentSection, TextContentSection, AssetContentSection. |
| `apps/web/components/dashboard/preview/BookmarkPreview::CloseButton` | apps/web/components/dashboard/preview/BookmarkPreview.tsx | all | component | Function component. Props: label, onClick, className. Renders: IconTooltip, Button, X. |
| `apps/web/components/dashboard/preview/BookmarkPreview::ContentLoading` | apps/web/components/dashboard/preview/BookmarkPreview.tsx | all | component | Function component. Hooks: useTranslation. Renders: div, p, Globe. |
| `apps/web/components/dashboard/preview/BookmarkPreview::DetailsTitle` | apps/web/components/dashboard/preview/BookmarkPreview.tsx | all | component | Function component. Props: bookmark. Hooks: useTranslation. Renders: p, Separator. |
| `apps/web/components/dashboard/preview/BookmarkPreview::LinkDetailsTitle` | apps/web/components/dashboard/preview/BookmarkPreview.tsx | all | component | Function component. Props: bookmark. Hooks: useLinkSection. Renders: DetailsTitle. |
| `apps/web/components/dashboard/preview/BookmarkPreview::LinkMetadata` | apps/web/components/dashboard/preview/BookmarkPreview.tsx | all | component | Function component. Props: bookmark, readOnly. Hooks: useTranslation, useLinkSection. Renders: div, span, SavedDate, User, Building, MetadataDate. |
| `apps/web/components/dashboard/preview/BookmarkPreview::MetadataDate` | apps/web/components/dashboard/preview/BookmarkPreview.tsx | all | component | Function component. Props: icon, date, format. Hooks: useTranslation, useRelativeTime, useState, useEffect. Renders: span, Tooltip, TooltipTrigger, Icon, TooltipPortal, TooltipContent. |
| `apps/web/components/dashboard/preview/BookmarkPreview::NavigationButtons` | apps/web/components/dashboard/preview/BookmarkPreview.tsx | all | component | Function component. Props: navigation, className. Hooks: useTranslation. Renders: IconTooltip, Button, ChevronLeft, ChevronRight. |
| `apps/web/components/dashboard/preview/BookmarkPreview::SavedDate` | apps/web/components/dashboard/preview/BookmarkPreview.tsx | all | component | Function component. Props: bookmark, readOnly. Hooks: useTranslation. Renders: div, MetadataDate, ArchivedStatus. |
| `apps/web/components/dashboard/preview/BookmarkPreview::ViewOriginalButton` | apps/web/components/dashboard/preview/BookmarkPreview.tsx | all | component | Function component. Props: url, className. Hooks: useTranslation. Renders: span, IconTooltip, Button, Link, ExternalLink. |
| `apps/web/components/dashboard/preview/content-renderers/AmazonRenderer::AmazonRendererComponent` | apps/web/components/dashboard/preview/content-renderers/AmazonRenderer.tsx | all | component | Function component. Props: bookmark. Renders: div, img, h2, p, span, a, ShoppingCart. |
| `apps/web/components/dashboard/preview/content-renderers/InstagramRenderer::InstagramRendererComponent` | apps/web/components/dashboard/preview/content-renderers/InstagramRenderer.tsx | all | component | Function component. Props: bookmark. Renders: div, iframe. |
| `apps/web/components/dashboard/preview/content-renderers/TikTokRenderer::TikTokRendererComponent` | apps/web/components/dashboard/preview/content-renderers/TikTokRenderer.tsx | all | component | Function component. Props: bookmark. Renders: div, iframe. |
| `apps/web/components/dashboard/preview/content-renderers/XRenderer::XRendererComponent` | apps/web/components/dashboard/preview/content-renderers/XRenderer.tsx | all | component | Function component. Props: bookmark. Renders: div, Tweet. |
| `apps/web/components/dashboard/preview/content-renderers/YouTubeRenderer::YouTubeRendererComponent` | apps/web/components/dashboard/preview/content-renderers/YouTubeRenderer.tsx | all | component | Function component. Props: bookmark. Renders: div, iframe. |
| `apps/web/components/dashboard/preview/HighlightsBox::HighlightsBox` | apps/web/components/dashboard/preview/HighlightsBox.tsx | all | component | Function component. Props: bookmarkId, readOnly. Hooks: useTRPC, useTranslation, useState, useQuery, useRef, useEffect. Renders: span, div, Separator, Collapsible, CollapsibleTrigger, ChevronRight, CollapsibleContent, HighlightCard. |
| `apps/web/components/dashboard/preview/IconControl::IconTooltip` | apps/web/components/dashboard/preview/IconControl.tsx | all | component | Function component. Props: label, side, children. Renders: Tooltip, TooltipTrigger, TooltipPortal, TooltipContent. |
| `apps/web/components/dashboard/preview/IconControl::RestoreTooltip` | apps/web/components/dashboard/preview/IconControl.tsx | all | component | Function component. Hooks: useTranslation. Renders: p. |
| `apps/web/components/dashboard/preview/LinkContentSection::CustomRendererErrorFallback` | apps/web/components/dashboard/preview/LinkContentSection.tsx | all | component | Function component. Props: error. Hooks: useTranslation. Renders: div, details, summary, code, Alert, AlertTriangle, AlertTitle, AlertDescription. |
| `apps/web/components/dashboard/preview/LinkContentSection::FullPageArchiveSection` | apps/web/components/dashboard/preview/LinkContentSection.tsx | all | component | Function component. Props: link. Renders: iframe. |
| `apps/web/components/dashboard/preview/LinkContentSection::LinkContentSection` | apps/web/components/dashboard/preview/LinkContentSection.tsx | all | component | Function component. Props: bookmark, toolbarSlot, compactToolbar, titleSlot, originalUrl, onShowContent. Hooks: useTranslation, useReaderSettings, useLinkSection, useRef, useCallback, useTitleScrolledAway, +1 more. Renders: div, p, ErrorBoundary, RendererComponent, ArticleTitleBlock, ReaderView, FullPageArchiveSection, VideoSection. |
| `apps/web/components/dashboard/preview/LinkContentSection::PDFSection` | apps/web/components/dashboard/preview/LinkContentSection.tsx | all | component | Function component. Props: link. Renders: iframe. |
| `apps/web/components/dashboard/preview/LinkContentSection::ScreenshotSection` | apps/web/components/dashboard/preview/LinkContentSection.tsx | all | component | Function component. Props: link. Renders: div, Image. |
| `apps/web/components/dashboard/preview/LinkContentSection::VideoSection` | apps/web/components/dashboard/preview/LinkContentSection.tsx | all | component | Function component. Props: link. Renders: div, video, source. |
| `apps/web/components/dashboard/preview/LinkViewMenu::LinkViewMenu` | apps/web/components/dashboard/preview/LinkViewMenu.tsx | all | component | Function component. Props: bookmark, link, section, availableRenderers, compact, columnRef, +4 more. Hooks: useTranslation, useSession, useClientConfig, useReaderSettings, useOfflineCopyActions, useRef, +1 more. Renders: span, a, DropdownMenu, IconTooltip, DropdownMenuTrigger, Button, CurrentIcon, ChevronDown. |
| `apps/web/components/dashboard/preview/NoteEditor::NoteEditor` | apps/web/components/dashboard/preview/NoteEditor.tsx | all | component | Function component. Props: bookmark, disabled. Hooks: useTranslation, useClientConfig, useNoteDraft. Renders: div, p, span, Textarea. |
| `apps/web/components/dashboard/preview/ReaderBarActions::ReaderBarActions` | apps/web/components/dashboard/preview/ReaderBarActions.tsx | all | component | Function component. Props: bookmark. Hooks: useTranslation, useFavouriteAndArchive. Renders: IconTooltip, ActionButton, LoadingSpinner, FavouritedActionIcon, RestoreTooltip, ArchivedActionIcon. |
| `apps/web/components/dashboard/preview/ReaderBarActions::ReaderMoreMenu` | apps/web/components/dashboard/preview/ReaderBarActions.tsx | all | component | Function component. Props: bookmark, className, onPrint, onShowHighlights. Hooks: useTranslation, useFavouriteAndArchive, useRef, useState. Renders: Popover, PopoverAnchor, DropdownMenu, IconTooltip, DropdownMenuTrigger, Button. |
| `apps/web/components/dashboard/preview/ReaderBarActions::TagsPopoverContent` | apps/web/components/dashboard/preview/ReaderBarActions.tsx | all | component | Function component. Props: bookmark, onCloseAutoFocus. Hooks: useRef. Renders: PopoverContent, BookmarkTagsEditor. |
| `apps/web/components/dashboard/preview/ReaderSettingsPopover::ReaderSettingsPopover` | apps/web/components/dashboard/preview/ReaderSettingsPopover.tsx | all | component | Function component. Props: open, onOpenChange, variant, columnRef, hideTrigger, anchorBottom, +1 more. Hooks: useTranslation, useRef, useReaderSettings. Renders: span, p, div, h3, label, Popover, PopoverAnchor, Tooltip, +3 more. |
| `apps/web/components/dashboard/preview/ReaderView::ReaderView` | apps/web/components/dashboard/preview/ReaderView.tsx | all | component | Function component. Props: bookmarkId, className, style, readOnly, progressBarStyle, progressBarClassName, +1 more. Hooks: useTranslation, useTRPC, useQuery, useReadingProgress, useQueryState, useRef, +4 more. Renders: div, h3, p, FullPageSpinner, BookmarkLoadError, FileX, ScrollProgressTracker, ReadingProgressBanner, +1 more. |
| `apps/web/components/dashboard/preview/ReadingProgressBanner::ReadingProgressBanner` | apps/web/components/dashboard/preview/ReadingProgressBanner.tsx | all | component | Function component. Props: percent, onContinue, onDismiss. Hooks: useTranslation. Renders: div, span, button, BookOpen, IconTooltip, X. |
| `apps/web/components/dashboard/preview/SavedPageOverview::Favicon` | apps/web/components/dashboard/preview/SavedPageOverview.tsx | all | component | Function component. Props: src. Hooks: useState, useCallback. Renders: Image. |
| `apps/web/components/dashboard/preview/SavedPageOverview::SavedPageOverview` | apps/web/components/dashboard/preview/SavedPageOverview.tsx | all | component | Function component. Props: link, title, onSelectSection. Hooks: useTranslation. Renders: div, article, span, h2, p, Image, Globe2, Favicon, +3 more. |
| `apps/web/components/dashboard/preview/TextContentSection::TextContentSection` | apps/web/components/dashboard/preview/TextContentSection.tsx | all | component | Function component. Props: bookmark, readOnly. Hooks: useTranslation, useState. Renders: div, ScrollArea, Image, ArticleTitleBlock, Button, Pencil, BookmarkedTextEditor. |
| `apps/web/components/dashboard/preview/UnavailableViewOption::UnavailableViewOption` | apps/web/components/dashboard/preview/UnavailableViewOption.tsx | all | component | Function component. Props: value, icon, label, reason, action. Renders: div, span, SelectItem, Icon. |
| `apps/web/components/dashboard/ReportProblemDialog::ReportProblemDialog` | apps/web/components/dashboard/ReportProblemDialog.tsx | all | component | Function component. Hooks: useTranslation, useTRPC, useSession, useTheme, useProblemReportStore, useState, +4 more. Renders: div, p, form, pre, Dialog, DialogContent, CheckCircle2, DialogTitle, +2 more. |
| `apps/web/components/dashboard/rules/RuleEngineActionBuilder::ActionBuilder` | apps/web/components/dashboard/rules/RuleEngineActionBuilder.tsx | all | component | Function component. Props: value, onChange. Hooks: useTranslation. Renders: div, p, Tag, List, Download, Star, Archive, Card. |
| `apps/web/components/dashboard/rules/RuleEngineConditionBuilder::ConditionBuilder` | apps/web/components/dashboard/rules/RuleEngineConditionBuilder.tsx | all | component | Function component. Props: value, onChange, eventType, level, onRemove. Hooks: useTranslation, useState. Renders: div, span, Link, Heading, Rss, FileType, Tag, Star. |
| `apps/web/components/dashboard/rules/RuleEngineEventSelector::EventSelector` | apps/web/components/dashboard/rules/RuleEngineEventSelector.tsx | all | component | Function component. Props: value, onChange. Hooks: useTranslation. Renders: div, Card, CardContent, Select, SelectTrigger, SelectValue, SelectContent. |
| `apps/web/components/dashboard/rules/RuleEngineRuleEditor::RuleEditor` | apps/web/components/dashboard/rules/RuleEngineRuleEditor.tsx | all | component | Function component. Props: rule, onCancel. Hooks: useTranslation, useCreateRule, useUpdateRule, useState, useEffect. Renders: form, div, Card, CardHeader, CardTitle, CardContent, Label, Input. |
| `apps/web/components/dashboard/rules/RuleEngineRuleList::RuleList` | apps/web/components/dashboard/rules/RuleEngineRuleList.tsx | all | component | Function component. Props: rules, onEditRule, onDeleteRule. Hooks: useTranslation, useClientConfig, useUpdateRule, useDeleteRule. Renders: div, h3, p, span, Card, CardContent, Switch, Button, +2 more. |
| `apps/web/components/dashboard/search/QueryExplainerTooltip::MatcherComp` | apps/web/components/dashboard/search/QueryExplainerTooltip.tsx | all | component | Function component. Props: matcher. Hooks: useTranslation. Renders: TableRow, TableCell, FormattedDate, Table, TableBody, MatcherComp. |
| `apps/web/components/dashboard/search/QueryExplainerTooltip::QueryExplainerTooltip` | apps/web/components/dashboard/search/QueryExplainerTooltip.tsx | all | component | Function component. Props: parsedSearchQuery, header, className, trigger. Hooks: useTranslation. Renders: Table, TableBody, TableRow, TableCell, MatcherComp, Tooltip. |
| `apps/web/components/dashboard/search/SearchInput::SearchInput` | apps/web/components/dashboard/search/SearchInput.tsx | all | component | Wrapped component. Props: className, onKeyDown, ...props. Hooks: useTranslation, useClientConfig, useDoBookmarkSearch, useSearchHistory, useState, useRef, +6 more. Renders: div, item.Icon, span, EditListModal, Button, Link, QueryExplainerTooltip, SearchModeSelector, +1 more. |
| `apps/web/components/dashboard/search/SearchModeSelector::SearchModeSelector` | apps/web/components/dashboard/search/SearchModeSelector.tsx | all | component | Function component. Props: value, onValueChange. Hooks: useTranslation. Renders: span, mode.Icon, DropdownMenu, DropdownMenuTrigger, Button, ActiveIcon, ChevronDown, DropdownMenuContent. |
| `apps/web/components/dashboard/sidebar/AllLists::AllLists` | apps/web/components/dashboard/sidebar/AllLists.tsx | all | component | Function component. Props: initialData. Hooks: useTranslation, usePathname, useCallback, useState, useBookmarkLists, useMemo, +1 more. Renders: ul, li, p, button, span, EditListModal, Plus, SidebarItem, +3 more. |
| `apps/web/components/dashboard/sidebar/AllLists::DroppableListSidebarItem` | apps/web/components/dashboard/sidebar/AllLists.tsx | all | component | Function component. Props: node, level, open, numBookmarks, selectedListId, setSelectedListId. Hooks: useTranslation, useDropTarget. Renders: span, SidebarItem, CollapsibleTriggerChevron, ListOptions, Button, MoreHorizontal. |
| `apps/web/components/dashboard/sidebar/InvitationNotificationBadge::InvitationNotificationBadge` | apps/web/components/dashboard/sidebar/InvitationNotificationBadge.tsx | all | component | Function component. Hooks: useTRPC, useQuery. Renders: div, span. |
| `apps/web/components/dashboard/SortOrderToggle::SortOrderToggle` | apps/web/components/dashboard/SortOrderToggle.tsx | all | component | Function component. Hooks: useTranslation, useInSearchPageStore, useBookmarkSearchState, useSortOrderStore, useEffect. Renders: div, span, DropdownMenu, Tooltip, TooltipTrigger, DropdownMenuTrigger, Button, ListFilter. |
| `apps/web/components/dashboard/tags/AllTagsView::AllTagsView` | apps/web/components/dashboard/tags/AllTagsView.tsx | all | component | Function component. Hooks: useTranslation, useQueryState, useDebounce, useState, useBulkTagActionsStore, useCallback, +3 more. Renders: div, p, span, Skeleton, Tag, MultiTagSelector, TagPill, DeleteTagConfirmationDialog, +1 more. |
| `apps/web/components/dashboard/tags/AllTagsView::DeleteAllUnusedTags` | apps/web/components/dashboard/tags/AllTagsView.tsx | all | component | Function component. Props: numUnusedTags. Hooks: useTranslation, useDeleteUnusedTags. Renders: ActionConfirmingDialog, ActionButton, Button. |
| `apps/web/components/dashboard/tags/BulkTagAction::BulkTagAction` | apps/web/components/dashboard/tags/BulkTagAction.tsx | all | component | Function component. Hooks: useTranslation, useBulkTagActionsStore, useState, useEffect, useDeleteTag. Renders: p, div, CheckCheck, Trash2, X, ActionConfirmingDialog, ActionButton, Toggle. |
| `apps/web/components/dashboard/tags/CreateTagModal::CreateTagModal` | apps/web/components/dashboard/tags/CreateTagModal.tsx | all | component | Function component. Hooks: useTranslation, useState, useForm, useCreateTag. Renders: form, div, Dialog, DialogTrigger, Button, Plus, DialogContent, Form. |
| `apps/web/components/dashboard/tags/DeleteTagConfirmationDialog::DeleteTagConfirmationDialog` | apps/web/components/dashboard/tags/DeleteTagConfirmationDialog.tsx | all | component | Function component. Props: tag, open, setOpen. Hooks: usePathname, useRouter, useDeleteTag. Renders: ActionConfirmingDialog, ActionButton. |
| `apps/web/components/dashboard/tags/EditableTagName::EditableTagName` | apps/web/components/dashboard/tags/EditableTagName.tsx | all | component | Function component. Props: tag, className. Hooks: useRouter, usePathname, useUpdateTag. Renders: EditableText. |
| `apps/web/components/dashboard/tags/MergeTagModal::MergeTagModal` | apps/web/components/dashboard/tags/MergeTagModal.tsx | all | component | Function component. Props: open, setOpen, tag, children. Hooks: usePathname, useTranslation, useRouter, useForm, useMergeTag. Renders: form, Dialog, DialogTrigger, DialogContent, Form, DialogHeader, DialogTitle. |
| `apps/web/components/dashboard/tags/MultiTagSelector::MultiTagSelector` | apps/web/components/dashboard/tags/MultiTagSelector.tsx | all | component | Wrapped component. Props: id, name, count. Hooks: useBulkTagActionsStore. Renders: div, button, span, Check. |
| `apps/web/components/dashboard/tags/RenameTagModal::RenameTagModal` | apps/web/components/dashboard/tags/RenameTagModal.tsx | all | component | Function component. Props: tag, open, setOpen. Hooks: useTranslation, useForm, useEffect, useUpdateTag. Renders: form, div, Dialog, DialogContent, Form, DialogHeader, DialogTitle, FormField. |
| `apps/web/components/dashboard/tags/TagAutocomplete::TagAutocomplete` | apps/web/components/dashboard/tags/TagAutocomplete.tsx | all | component | Function component. Props: tagId, onChange, className. Hooks: useTRPC, useState, useDebounce, useTagAutocomplete, useQuery. Renders: div, span, LoadingSpinner, Popover, PopoverTrigger, Button, X, ChevronsUpDown. |
| `apps/web/components/dashboard/tags/TagAutocomplete::TagNamePicker` | apps/web/components/dashboard/tags/TagAutocomplete.tsx | all | component | Function component. Props: id, placeholder, selectedNames, onToggle, getTypedNameLabel. Hooks: useTranslation, useState, useDebounce, useRef, useTagAutocomplete. Renders: button, span, Popover, PopoverTrigger, ChevronDown, PopoverContent, Command, CommandInput. |
| `apps/web/components/dashboard/tags/TagHeader::TagHeader` | apps/web/components/dashboard/tags/TagHeader.tsx | all | component | Function component. Props: initialData. Hooks: useTRPC, useTranslation, useRouter, useQuery. Renders: div, span, h1, Hash, User, Bot, TagOptions, Button, +1 more. |
| `apps/web/components/dashboard/tags/TagOptions::TagOptions` | apps/web/components/dashboard/tags/TagOptions.tsx | all | component | Function component. Props: tag, children. Hooks: useTranslation, useShowArchived, useState, useRef. Renders: span, DropdownMenu, DeleteTagConfirmationDialog, MergeTagModal, RenameTagModal, DropdownMenuTrigger, DropdownMenuContent. |
| `apps/web/components/dashboard/tags/TagPill::TagPill` | apps/web/components/dashboard/tags/TagPill.tsx | all | component | Wrapped component. Props: id, name, count, isDraggable, onOpenDialog. Hooks: useState, useRef, useMergeTag, useDragAndDrop. Renders: div, span, Link, Button, X, Draggable. |
| `apps/web/components/dashboard/UploadDropzone::UploadDropzone` | apps/web/components/dashboard/UploadDropzone.tsx | all | component | Function component. Props: children. Hooks: useState, useTranslation, useUploadAssets. Renders: div, input, p, DropZone, LoadingSpinner. |
| `apps/web/components/dashboard/ViewOptions::ViewOptions` | apps/web/components/dashboard/ViewOptions.tsx | all | component | Function component. Hooks: useTranslation, useBookmarkLayout, useGridColumns, useBookmarkDisplaySettings, useState, useTransition, +2 more. Renders: span, div, DropdownMenu, Tooltip, TooltipTrigger, DropdownMenuTrigger, Button, Settings. |
| `apps/web/components/DemoModeBanner::DemoModeBanner` | apps/web/components/DemoModeBanner.tsx | all | component | Function component. Renders: div. |
| `apps/web/components/invite/InviteAcceptForm::InviteAcceptForm` | apps/web/components/invite/InviteAcceptForm.tsx | all | component | Function component. Props: token. Hooks: useTRPC, useRouter, useForm, useState, useQuery, useEffect, +1 more. Renders: div, p, form, Card, CardHeader, CardTitle, CardDescription, CardContent, +1 more. |
| `apps/web/components/KarakeepIcon::KarakeepLogo` | apps/web/components/KarakeepIcon.tsx | all | component | Function component. Props: height. Renders: span, KarakeepFull. |
| `apps/web/components/public/lists/PublicBookmarkGrid::BookmarkCard` | apps/web/components/public/lists/PublicBookmarkGrid.tsx | all | component | Function component. Props: bookmark. Hooks: useTranslation. Renders: div, h3, span, BookmarkMarkdownComponent, PublicCardImage, ImageIcon, FileIcon, Link, +1 more. |
| `apps/web/components/public/lists/PublicBookmarkGrid::ExpandNote` | apps/web/components/public/lists/PublicBookmarkGrid.tsx | all | component | Function component. Props: bookmark, children. Hooks: useTranslation. Renders: Dialog, Tooltip, TooltipTrigger, DialogTrigger, Button, Expand. |
| `apps/web/components/public/lists/PublicBookmarkGrid::PublicBookmarkGrid` | apps/web/components/public/lists/PublicBookmarkGrid.tsx | all | component | Function component. Props: bookmarks, nextCursor, list. Hooks: useTRPC, useTranslation, useInView, useInfiniteQuery, useEffect, useMemo. Renders: div, Masonry, BookmarkCard, ActionButton. |
| `apps/web/components/public/lists/PublicBookmarkGrid::PublicCardImage` | apps/web/components/public/lists/PublicBookmarkGrid.tsx | all | component | Function component. Props: href, src. Renders: Link, CardImage. |
| `apps/web/components/public/lists/PublicBookmarkGrid::TagPill` | apps/web/components/public/lists/PublicBookmarkGrid.tsx | all | component | Function component. Props: tag. Renders: div. |
| `apps/web/components/public/lists/PublicListHeader::PublicListHeader` | apps/web/components/public/lists/PublicListHeader.tsx | all | component | Function component. Props: list. Hooks: useTranslation. Renders: div, span, h1, p, KarakeepLogo, ButtonWithTooltip, Link, RssIcon. |
| `apps/web/components/settings/AddApiKey::AddApiKey` | apps/web/components/settings/AddApiKey.tsx | all | component | Function component. Props: isAdmin. Hooks: useTranslation, useRouter, useState, useEffect. Renders: Dialog, DialogTrigger, Button, Plus, DialogContent, DialogHeader. |
| `apps/web/components/settings/AddApiKey::AddApiKeyForm` | apps/web/components/settings/AddApiKey.tsx | all | component | Function component. Props: isAdmin, onSuccess. Hooks: useTRPC, useTranslation, useState, useMutation, useForm, useClientConfig. Renders: form, div, h3, p, Form, DialogBody, FormField, FormItem, +2 more. |
| `apps/web/components/settings/AddApiKey::ScopeCard` | apps/web/components/settings/AddApiKey.tsx | all | component | Function component. Props: id, value, label, description. Renders: span, Label, RadioGroupItem. |
| `apps/web/components/settings/AddApiKey::ScopeChoiceRow` | apps/web/components/settings/AddApiKey.tsx | all | component | Function component. Props: option, value, disabled, onChange. Hooks: useTranslation. Renders: div, p, RadioGroup, Label, RadioGroupItem. |
| `apps/web/components/settings/AISettings::AIPreferences` | apps/web/components/settings/AISettings.tsx | all | component | Function component. Hooks: useTranslation, useClientConfig, useUserSettings, useSavedField, useUpdateUserSettings, useForm, +1 more. Renders: form, SettingsSection, SavedHint, SettingsRows, Controller, SettingsRow, FieldLabel. |
| `apps/web/components/settings/AISettings::AISettings` | apps/web/components/settings/AISettings.tsx | all | component | Function component. Hooks: useTranslation. Renders: SettingsPage, AIPreferences, TagStyleSelector, CuratedTagsSelector, TaggingRules, PromptDemo. |
| `apps/web/components/settings/AISettings::CuratedTagsSelector` | apps/web/components/settings/AISettings.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useUserSettings, useSavedField, useUpdateUserSettings, useCallback, +6 more. Renders: SettingsSection, SavedHint, TagsEditor. |
| `apps/web/components/settings/AISettings::PromptDemo` | apps/web/components/settings/AISettings.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQuery, useUserSettings, useClientConfig, useCallback. Renders: div, p, code, SettingsSection. |
| `apps/web/components/settings/AISettings::PromptEditor` | apps/web/components/settings/AISettings.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQueryClient, useForm, useFormErrors, useMutation. Renders: form, Form, FormField, FormItem, FormControl, Input, FormMessage. |
| `apps/web/components/settings/AISettings::PromptRow` | apps/web/components/settings/AISettings.tsx | all | component | Function component. Props: prompt. Hooks: useTRPC, useTranslation, useQueryClient, useSavedField, useMutation, useForm, +1 more. Renders: form, Form, FormField, FormItem, FormControl, Input, FormMessage. |
| `apps/web/components/settings/AISettings::TaggingRules` | apps/web/components/settings/AISettings.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQuery. Renders: div, SettingsSection, Empty, EmptyHeader, EmptyMedia, ScrollText, EmptyTitle. |
| `apps/web/components/settings/AISettings::TagStyleSelector` | apps/web/components/settings/AISettings.tsx | all | component | Function component. Hooks: useTranslation, useUserSettings, useAutosavedSettings. Renders: div, SettingsSection, SavedHint, RadioGroup, FieldLabel, Field, FieldContent. |
| `apps/web/components/settings/ApiKeyRowActions::ApiKeyRowActions` | apps/web/components/settings/ApiKeyRowActions.tsx | all | component | Function component. Props: name, id. Hooks: useTranslation, useState. Renders: RegenerateApiKey, DeleteApiKey, RowActionsMenu, RefreshCcw, Trash2. |
| `apps/web/components/settings/ApiKeySettings::ApiKeys` | apps/web/components/settings/ApiKeySettings.tsx | all | component | Function component. Props: isAdmin, keys. Hooks: useTranslation. Renders: span, div, Empty, EmptyHeader, EmptyMedia, KeyRound, EmptyTitle, EmptyDescription. |
| `apps/web/components/settings/ApiKeySuccess::ApiKeySuccess` | apps/web/components/settings/ApiKeySuccess.tsx | all | component | Function component. Props: apiKey, note. Hooks: useTranslation, useState, useRef, useEffect. Renders: div, p, span, AlertTriangle, Input, Button, Check, Copy. |
| `apps/web/components/settings/BackupSettings::BackupConfigurationForm` | apps/web/components/settings/BackupSettings.tsx | all | component | Function component. Hooks: useTranslation, useClientConfig, useUserSettings, useSavedField, useUpdateUserSettings, useForm, +3 more. Renders: form, div, SavedHint, SettingsSection, Form, SettingsRows, FormField, FormItem. |
| `apps/web/components/settings/BackupSettings::BackupRow` | apps/web/components/settings/BackupSettings.tsx | all | component | Function component. Props: backup. Hooks: useTRPC, useTranslation, useQueryClient, useState, useMutation. Renders: span, div, TableRow, TableCell, FormattedDate, StackedLabel, CheckCircle, Tooltip. |
| `apps/web/components/settings/BackupSettings::BackupSettings` | apps/web/components/settings/BackupSettings.tsx | all | component | Function component. Renders: BackupConfigurationForm, BackupsList. |
| `apps/web/components/settings/BackupSettings::BackupsList` | apps/web/components/settings/BackupSettings.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQueryClient, useQuery, useMutation. Renders: span, ActionButton, Play, SettingsSection, Trans, Link, FullPageSpinner. |
| `apps/web/components/settings/ChangePassword::ChangePassword` | apps/web/components/settings/ChangePassword.tsx | all | component | Function component. Hooks: useTranslation, useForm, useSavedField, useMutation. Renders: form, SettingsSection, Form, SettingsRows, FormField, FormItem, SettingsRow. |
| `apps/web/components/settings/DeleteAccount::DeleteAccount` | apps/web/components/settings/DeleteAccount.tsx | all | component | Function component. Hooks: useTranslation, useRouter, useState, useWhoAmI, useForm, useDeleteAccount. Renders: div, p, form, SettingsSection, ActionConfirmingDialog, AlertTriangle, Alert, AlertDescription, +1 more. |
| `apps/web/components/settings/DeleteApiKey::DeleteApiKey` | apps/web/components/settings/DeleteApiKey.tsx | all | component | Function component. Props: name, id, open, setOpen. Hooks: useTRPC, useTranslation, useRouter, useMutation. Renders: ActionConfirmingDialog, ActionButton. |
| `apps/web/components/settings/FeedSettings::EditFeedDialog` | apps/web/components/settings/FeedSettings.tsx | all | component | Function component. Props: feed, open, setOpen. Hooks: useTRPC, useTranslation, useQueryClient, useEffect, useMutation, useForm, +1 more. Renders: form, div, Dialog, DialogContent, DialogHeader, DialogTitle, DialogBody, Form. |
| `apps/web/components/settings/FeedSettings::FeedRow` | apps/web/components/settings/FeedSettings.tsx | all | component | Function component. Props: feed. Hooks: useTRPC, useTranslation, useQueryClient, useState, useMutation. Renders: span, div, TableRow, TableCell, Link, StackedLabel, FormattedDate, CheckCircle. |
| `apps/web/components/settings/FeedSettings::FeedsEditorDialog` | apps/web/components/settings/FeedSettings.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useState, useQueryClient, useForm, useFeedFormErrors, +2 more. Renders: form, div, Dialog, DialogTrigger, Button, Plus, DialogContent, DialogHeader. |
| `apps/web/components/settings/FeedSettings::FeedSettings` | apps/web/components/settings/FeedSettings.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQuery. Renders: span, SettingsPage, FeedsEditorDialog, FullPageSpinner, Empty, EmptyHeader, EmptyMedia. |
| `apps/web/components/settings/ImportExport::ExportSection` | apps/web/components/settings/ImportExport.tsx | all | component | Function component. Hooks: useTranslation, useState, useQueryClient, useQuery, useEffect, useCallback. Renders: SettingsSection, SettingsRow, Label, Select, SelectTrigger, SelectValue. |
| `apps/web/components/settings/ImportExport::ImportExport` | apps/web/components/settings/ImportExport.tsx | all | component | Function component. Hooks: useTranslation. Renders: SettingsPage, ExportSection, ImportSection, ImportSessionsSection. |
| `apps/web/components/settings/ImportExport::ImportProviderRow` | apps/web/components/settings/ImportExport.tsx | all | component | Function component. Props: name, accept, isFileInvalid, onFileSelect. Hooks: useTranslation, useRef. Renders: li, button, span, div, p, a, Upload, AlertCircle. |
| `apps/web/components/settings/ImportExport::ImportSection` | apps/web/components/settings/ImportExport.tsx | all | component | Function component. Hooks: useTranslation, useBookmarkImport, useState, useMemo. Renders: ul, div, p, SettingsSection, Alert, AlertCircle, AlertTitle, AlertDescription, +1 more. |
| `apps/web/components/settings/ImportSessionCard::ImportSessionCard` | apps/web/components/settings/ImportSessionCard.tsx | all | component | Function component. Props: session. Hooks: useTranslation, useImportSessionStats, useDeleteImportSession, useFinalizeImportStaging, usePauseImportSession, useResumeImportSession. Renders: div, h3, p, span, h4, Card, CardHeader, Badge, +3 more. |
| `apps/web/components/settings/ImportSessionDetail::ImportSessionDetail` | apps/web/components/settings/ImportSessionDetail.tsx | all | component | Function component. Props: sessionId. Hooks: useTranslation, useRouter, useState, useImportSessionStats, useImportSessionResults, useDeleteImportSession, +5 more. Renders: div, span, h4, p, FullPageSpinner, Link, ArrowLeft, PageHeader, +2 more. |
| `apps/web/components/settings/ImportSessionsSection::ImportSessionsSection` | apps/web/components/settings/ImportSessionsSection.tsx | all | component | Function component. Hooks: useTranslation, useListImportSessions. Renders: div, SettingsSection, FullPageSpinner, Empty, EmptyHeader, EmptyTitle, ImportSessionCard. |
| `apps/web/components/settings/Maintenance::MaintenanceError` | apps/web/components/settings/Maintenance.tsx | all | component | Function component. Props: onRetry. Hooks: useTranslation. Renders: div, p, Button. |
| `apps/web/components/settings/Maintenance::MaintenanceSearch` | apps/web/components/settings/Maintenance.tsx | all | component | Function component. Props: props: ComponentProps. Renders: div, Input, ListFilter. |
| `apps/web/components/settings/Maintenance::SelectionCheckbox` | apps/web/components/settings/Maintenance.tsx | all | component | Function component. Props: indeterminate, insideLabel, className, ...props. Hooks: useRef, useEffect. Renders: input, label. |
| `apps/web/components/settings/ProfileNameForm::ProfileNameForm` | apps/web/components/settings/ProfileNameForm.tsx | all | component | Function component. Props: name. Hooks: useTranslation, useRouter, useSession, useSavedField, useForm, useUpdateUserProfile. Renders: form, Form, FormField, FormItem, SettingsRow, FormLabel, SavedHint. |
| `apps/web/components/settings/ReadingSettings::ReadingSettings` | apps/web/components/settings/ReadingSettings.tsx | all | component | Function component. Hooks: useTranslation, useClientConfig, useReaderSettings, useState, useSavedField. Renders: div, p, ul, li, SavedHint, Alert, AlertTriangle, AlertDescription, +2 more. |
| `apps/web/components/settings/RegenerateApiKey::RegenerateApiKey` | apps/web/components/settings/RegenerateApiKey.tsx | all | component | Function component. Props: id, name, open, setOpen. Hooks: useTRPC, useTranslation, useRouter, useState, useMutation. Renders: p, Dialog, DialogContent, DialogHeader, DialogTitle, DialogDescription, ApiKeySuccess. |
| `apps/web/components/settings/RowActions::RowActionsMenu` | apps/web/components/settings/RowActions.tsx | all | component | Function component. Props: items, label, disabledReason, className. Hooks: useTranslation, useRef. Renders: span, RowIconButton, MoreHorizontal, DropdownMenu, Tooltip, TooltipTrigger, DropdownMenuTrigger. |
| `apps/web/components/settings/RowActions::RowIconButton` | apps/web/components/settings/RowActions.tsx | all | component | Wrapped component. Props: label, destructive, disabledReason, className, ...props. Renders: Tooltip, TooltipTrigger, Button, TooltipPortal, TooltipContent, ButtonWithTooltip. |
| `apps/web/components/settings/SaveBar::SaveBar` | apps/web/components/settings/SaveBar.tsx | all | component | Function component. Props: saving, saveLabel, onDiscard. Hooks: useTranslation, useRef, useState, useLayoutEffect. Renders: div, span, Button, ActionButton. |
| `apps/web/components/settings/SavedHint::SavedHint` | apps/web/components/settings/SavedHint.tsx | all | component | Function component. Props: show, failed. Hooks: useTranslation. Renders: span, AlertCircle, Check. |
| `apps/web/components/settings/SectionNav::SectionIndex` | apps/web/components/settings/SectionNav.tsx | all | component | Function component. Props: title, groups, desktopPath. Hooks: useRouter, useEffect. Renders: div, section, h2, ul, li, span, PageHeader, Link, +1 more. |
| `apps/web/components/settings/SectionNav::SectionMobileBar` | apps/web/components/settings/SectionNav.tsx | all | component | Function component. Props: indexPath, indexLabel, backToAppLabel. Hooks: usePathname. Renders: nav, Link, ChevronLeft, Home. |
| `apps/web/components/settings/SectionSidebar::SectionSidebar` | apps/web/components/settings/SectionSidebar.tsx | all | component | Function component. Props: groups. Hooks: useTranslation. Renders: aside, ul, div, h2, SidebarItem, ArrowLeft, SidebarVersion. |
| `apps/web/components/settings/SettingsPage::SettingsFormFooter` | apps/web/components/settings/SettingsPage.tsx | all | component | Function component. Props: children. Renders: div. |
| `apps/web/components/settings/SettingsPage::SettingsPage` | apps/web/components/settings/SettingsPage.tsx | all | component | Function component. Props: title, description, action, children. Renders: div, PageHeader. |
| `apps/web/components/settings/SettingsPage::SettingsRow` | apps/web/components/settings/SettingsPage.tsx | all | component | Function component. Props: label, description, hint, inline, children. Renders: div, p. |
| `apps/web/components/settings/SettingsPage::SettingsRows` | apps/web/components/settings/SettingsPage.tsx | all | component | Function component. Props: children. Renders: div. |
| `apps/web/components/settings/SettingsPage::SettingsSection` | apps/web/components/settings/SettingsPage.tsx | all | component | Function component. Props: id, title, count, description, action, children. Renders: div, Card, CardHeader, CardTitle, Badge, CardDescription, CardContent. |
| `apps/web/components/settings/SubscriptionSettings::SubscriptionSettings` | apps/web/components/settings/SubscriptionSettings.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useClientConfig, useState, useQuery, useMutation, +1 more. Renders: div, label, p, h3, ul, li, Badge, SettingsSection, +4 more. |
| `apps/web/components/settings/UserAvatar::UserAvatar` | apps/web/components/settings/UserAvatar.tsx | all | component | Function component. Hooks: useTranslation, useRef, useWhoAmI, useUpdateUserAvatar, useUpload. Renders: div, span, input, p, SettingsRow, UserAvatarImage, ActionButton, Upload, +2 more. |
| `apps/web/components/settings/UserDetails::UserDetails` | apps/web/components/settings/UserDetails.tsx | all | component | Function component. Hooks: useTranslation. Renders: SettingsSection, SettingsRows, UserAvatar, SettingsRow, Label, Input. |
| `apps/web/components/settings/UserOptions::LanguageSelect` | apps/web/components/settings/UserOptions.tsx | all | component | Arrow function component. Props: onSaved, onFailed. Hooks: useInterfaceLang. Renders: Select, SelectTrigger, SelectValue, SelectContent, SelectItem. |
| `apps/web/components/settings/UserOptions::ThemeSelect` | apps/web/components/settings/UserOptions.tsx | all | component | Arrow function component. Props: onSaved. Hooks: useTranslation, useTheme, useState, useEffect. Renders: span, Select, SelectTrigger, SelectValue, SelectContent, SelectItem, Icon. |
| `apps/web/components/settings/UserOptions::UserOptions` | apps/web/components/settings/UserOptions.tsx | all | component | Function component. Hooks: useTranslation, useClientConfig, useUserSettings, useAutosavedSettings, useState, useEffect. Renders: SavedHint, SettingsSection, SettingsRows, SettingsRow, Label, ThemeSelect. |
| `apps/web/components/settings/WebhookEventSelector::WebhookEventSelector` | apps/web/components/settings/WebhookEventSelector.tsx | all | component | Function component. Props: value, onChange, ...triggerAttributes. Hooks: useTranslation. Renders: button, span, Popover, PopoverTrigger, ChevronDown, PopoverContent, Command, CommandInput. |
| `apps/web/components/settings/WebhookSettings::EditTokenDialog` | apps/web/components/settings/WebhookSettings.tsx | all | component | Function component. Props: webhook, open, setOpen. Hooks: useTRPC, useTranslation, useQueryClient, useEffect, useForm, useWebhookFormErrors, +1 more. Renders: form, Dialog, DialogContent, DialogHeader, DialogTitle, Form, FormField. |
| `apps/web/components/settings/WebhookSettings::EditWebhookDialog` | apps/web/components/settings/WebhookSettings.tsx | all | component | Function component. Props: webhook, open, setOpen. Hooks: useTRPC, useTranslation, useQueryClient, useEffect, useMutation, useForm, +1 more. Renders: form, Dialog, DialogContent, DialogHeader, DialogTitle, DialogBody, Form. |
| `apps/web/components/settings/WebhookSettings::WebhookPayloadExample` | apps/web/components/settings/WebhookSettings.tsx | all | component | Function component. Hooks: useTranslation. Renders: details, summary, pre. |
| `apps/web/components/settings/WebhookSettings::WebhookRow` | apps/web/components/settings/WebhookSettings.tsx | all | component | Function component. Props: webhook. Hooks: useTRPC, useTranslation, useQueryClient, useState, useMutation. Renders: div, TableRow, TableCell, StackedLabel, EditWebhookDialog, EditTokenDialog, ActionConfirmingDialog. |
| `apps/web/components/settings/WebhookSettings::WebhooksEditorDialog` | apps/web/components/settings/WebhookSettings.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useState, useQueryClient, useForm, useWebhookFormErrors, +2 more. Renders: form, Dialog, DialogTrigger, Button, Plus, DialogContent, DialogHeader. |
| `apps/web/components/settings/WebhookSettings::WebhookSettings` | apps/web/components/settings/WebhookSettings.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQuery. Renders: span, SettingsPage, WebhooksEditorDialog, FullPageSpinner, Empty, EmptyHeader, EmptyMedia. |
| `apps/web/components/shared/sidebar/MobileSidebar::MobileSidebar` | apps/web/components/shared/sidebar/MobileSidebar.tsx | all | component | Function component. Props: items. Hooks: useTranslation. Renders: aside, ul, MobileSidebarItem. |
| `apps/web/components/shared/sidebar/ModileSidebarItem::MobileSidebarItem` | apps/web/components/shared/sidebar/ModileSidebarItem.tsx | all | component | Function component. Props: name, logo, path. Hooks: usePathname. Renders: li, Link. |
| `apps/web/components/shared/sidebar/Sidebar::Sidebar` | apps/web/components/shared/sidebar/Sidebar.tsx | all | component | Function component. Props: items, extraSections. Hooks: useTranslation. Renders: aside, div, ul, SidebarItem, SidebarVersion. |
| `apps/web/components/shared/sidebar/SidebarItem::SidebarItem` | apps/web/components/shared/sidebar/SidebarItem.tsx | all | component | Function component. Props: name, logo, path, className, linkClassName, style, +8 more. Hooks: usePathname. Renders: li, div, span, Link. |
| `apps/web/components/shared/sidebar/SidebarLayout::SidebarLayout` | apps/web/components/shared/sidebar/SidebarLayout.tsx | all | component | Function component. Props: children, mobileSidebar, sidebar, modal. Renders: div, main, Header, ValidAccountCheck, DemoModeBanner, Separator, ErrorBoundary, ErrorFallback. |
| `apps/web/components/shared/sidebar/SidebarSectionHeading::SidebarSectionHeading` | apps/web/components/shared/sidebar/SidebarSectionHeading.tsx | all | component | Function component. Props: children, className. Renders: h2. |
| `apps/web/components/shared/sidebar/SidebarVersion::SidebarVersion` | apps/web/components/shared/sidebar/SidebarVersion.tsx | all | component | Function component. Props: serverVersion, changeLogVersion. Hooks: useClientConfig, useTranslation, useMemo, useState, useQuery, useEffect, +1 more. Renders: div, button, span, p, Link, Dialog, DialogContent, DialogHeader, +2 more. |
| `apps/web/components/shared/sidebar/SmartListMarker::SmartListMarker` | apps/web/components/shared/sidebar/SmartListMarker.tsx | all | component | Function component. Props: query. Hooks: useTranslation. Renders: span, Tooltip, TooltipTrigger, Sparkles, TooltipPortal, TooltipContent. |
| `apps/web/components/signin/ForgotPasswordForm::ForgotPasswordForm` | apps/web/components/signin/ForgotPasswordForm.tsx | all | component | Function component. Hooks: useState, useRouter, useForm. Renders: div, form, Card, CardHeader, CardTitle, CardDescription, CardContent, CheckCircle. |
| `apps/web/components/signin/OAuthAutoRedirect::OAuthAutoRedirect` | apps/web/components/signin/OAuthAutoRedirect.tsx | all | component | Function component. Props: oauthProviderId, redirectUrl. Hooks: useClientConfig, useSearchParams, useState, useEffect. Renders: div, span. |
| `apps/web/components/signin/ResetPasswordForm::ResetPasswordForm` | apps/web/components/signin/ResetPasswordForm.tsx | all | component | Function component. Props: token. Hooks: useState, useRouter, useForm. Renders: div, form, Card, CardHeader, CardTitle, CardDescription, CardContent, CheckCircle. |
| `apps/web/components/signin/SignInForm::SignInForm` | apps/web/components/signin/SignInForm.tsx | all | component | Function component. Props: redirectUrl. Renders: div, p, span, OAuthAutoRedirect, Card, CardHeader, CardTitle, CardDescription, +1 more. |
| `apps/web/components/signin/SignInProviderButton::SignInProviderButton` | apps/web/components/signin/SignInProviderButton.tsx | all | component | Function component. Props: provider, redirectUrl. Renders: Button. |
| `apps/web/components/signup/SignUpForm::SignUpForm` | apps/web/components/signup/SignUpForm.tsx | all | component | Function component. Props: redirectUrl. Hooks: useForm, useState, useRouter, useClientConfig, useRef. Renders: div, form, p, Card, CardHeader, CardTitle, CardDescription, CardContent, +1 more. |
| `apps/web/components/subscription/QuotaProgress::QuotaProgress` | apps/web/components/subscription/QuotaProgress.tsx | all | component | Function component. Hooks: useTRPC, useTranslation, useQuery. Renders: div, Card, CardHeader, CardTitle, CardDescription, CardContent, QuotaProgressItem. |
| `apps/web/components/subscription/QuotaProgress::QuotaProgressItem` | apps/web/components/subscription/QuotaProgress.tsx | all | component | Function component. Props: title, icon, used, quota, unlimited, formatter, +1 more. Hooks: useTranslation. Renders: div, h4, span, Progress. |
| `apps/web/components/theme-provider::ThemeProvider` | apps/web/components/theme-provider.tsx | all | component | Function component. Props: children, ...props. Renders: NextThemesProvider. |
| `apps/web/components/ui/action-button::ActionButton` | apps/web/components/ui/action-button.tsx | all | component | Wrapped component. Props: children, loading, spinner, disabled, ignoreDemoMode, ...props. Hooks: useClientConfig. Renders: LoadingSpinner, Button. |
| `apps/web/components/ui/action-button::ActionButtonWithTooltip` | apps/web/components/ui/action-button.tsx | all | component | Wrapped component. Props: tooltip, delayDuration, ...props. Renders: Tooltip, TooltipTrigger, ActionButton, TooltipPortal, TooltipContent. |
| `apps/web/components/ui/action-confirming-dialog::ActionConfirmingDialog` | apps/web/components/ui/action-confirming-dialog.tsx | all | component | Function component. Props: title, description, actionButton, children, onCloseAutoFocus, open, +1 more. Hooks: useTranslation, useState. Renders: div, Dialog, DialogTrigger, DialogContent, DialogHeader, DialogTitle, DialogDescription. |
| `apps/web/components/ui/alert::Alert` | apps/web/components/ui/alert.tsx | all | component | Wrapped component. Props: className, variant, ...props. Renders: div. |
| `apps/web/components/ui/alert::AlertDescription` | apps/web/components/ui/alert.tsx | all | component | Wrapped component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/alert::AlertTitle` | apps/web/components/ui/alert.tsx | all | component | Wrapped component. Props: className, ...props. Renders: h5. |
| `apps/web/components/ui/avatar::Avatar` | apps/web/components/ui/avatar.tsx | all | component | Wrapped component. Props: className, ...props. Renders: AvatarPrimitive.Root. |
| `apps/web/components/ui/avatar::AvatarFallback` | apps/web/components/ui/avatar.tsx | all | component | Wrapped component. Props: className, ...props. Renders: AvatarPrimitive.Fallback. |
| `apps/web/components/ui/avatar::AvatarImage` | apps/web/components/ui/avatar.tsx | all | component | Wrapped component. Props: className, ...props. Renders: AvatarPrimitive.Image. |
| `apps/web/components/ui/back-button::BackButton` | apps/web/components/ui/back-button.tsx | all | component | Function component. Props: ...props. Hooks: useRouter. Renders: Button. |
| `apps/web/components/ui/badge::Badge` | apps/web/components/ui/badge.tsx | all | component | Function component. Props: className, variant, ...props. Renders: div. |
| `apps/web/components/ui/button::Button` | apps/web/components/ui/button.tsx | all | component | Wrapped component. Props: variant, size, className, ...props. Renders: BaseButton. |
| `apps/web/components/ui/button::ButtonWithTooltip` | apps/web/components/ui/button.tsx | all | component | Wrapped component. Props: tooltip, delayDuration, shortcut, ...props. Renders: span, Tooltip, TooltipTrigger, Button, TooltipPortal, TooltipContent. |
| `apps/web/components/ui/calendar::Calendar` | apps/web/components/ui/calendar.tsx | all | component | Function component. Props: className, classNames, showOutsideDays, captionLayout, startMonth, endMonth, +4 more. Renders: div, td, DayPicker, ChevronLeftIcon, ChevronRightIcon, ChevronDownIcon. |
| `apps/web/components/ui/calendar::CalendarDayButton` | apps/web/components/ui/calendar.tsx | all | component | Function component. Props: className, day, modifiers, ...props. Hooks: useRef, useEffect. Renders: Button. |
| `apps/web/components/ui/card::Card` | apps/web/components/ui/card.tsx | all | component | Wrapped component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/card::CardContent` | apps/web/components/ui/card.tsx | all | component | Wrapped component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/card::CardDescription` | apps/web/components/ui/card.tsx | all | component | Wrapped component. Props: className, ...props. Renders: p. |
| `apps/web/components/ui/card::CardFooter` | apps/web/components/ui/card.tsx | all | component | Wrapped component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/card::CardHeader` | apps/web/components/ui/card.tsx | all | component | Wrapped component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/card::CardTitle` | apps/web/components/ui/card.tsx | all | component | Wrapped component. Props: className, ...props. Renders: h3. |
| `apps/web/components/ui/collapsible::CollapsibleTriggerChevron` | apps/web/components/ui/collapsible.tsx | all | component | Function component. Props: open, className. Renders: CollapsibleTrigger, ChevronRight. |
| `apps/web/components/ui/collapsible::CollapsibleTriggerTriangle` | apps/web/components/ui/collapsible.tsx | all | component | Function component. Props: open, className. Renders: CollapsibleTrigger, Triangle. |
| `apps/web/components/ui/command::Command` | apps/web/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: CommandPrimitive. |
| `apps/web/components/ui/command::CommandDialog` | apps/web/components/ui/command.tsx | all | component | Arrow function component. Props: children, ...props. Renders: Dialog, DialogContent, Command. |
| `apps/web/components/ui/command::CommandEmpty` | apps/web/components/ui/command.tsx | all | component | Wrapped component. Renders: CommandPrimitive.Empty. |
| `apps/web/components/ui/command::CommandGroup` | apps/web/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: CommandPrimitive.Group. |
| `apps/web/components/ui/command::CommandInput` | apps/web/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: div, Search, CommandPrimitive.Input. |
| `apps/web/components/ui/command::CommandItem` | apps/web/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: CommandPrimitive.Item. |
| `apps/web/components/ui/command::CommandList` | apps/web/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: CommandPrimitive.List. |
| `apps/web/components/ui/command::CommandSeparator` | apps/web/components/ui/command.tsx | all | component | Wrapped component. Props: className, ...props. Renders: CommandPrimitive.Separator. |
| `apps/web/components/ui/command::CommandShortcut` | apps/web/components/ui/command.tsx | all | component | Arrow function component. Props: className, ...props. Renders: span. |
| `apps/web/components/ui/copy-button::CopyBtn` | apps/web/components/ui/copy-button.tsx | all | component | Function component. Props: className, getStringToCopy. Hooks: useState, useEffect. Renders: button, Check, Copy. |
| `apps/web/components/ui/copy-button::CopyBtnV2` | apps/web/components/ui/copy-button.tsx | all | component | Function component. Props: className, getStringToCopy. Hooks: useState. Renders: Button, Check, Copy. |
| `apps/web/components/ui/dialog::DialogBody` | apps/web/components/ui/dialog.tsx | all | component | Arrow function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/dialog::DialogContent` | apps/web/components/ui/dialog.tsx | all | component | Wrapped component. Props: className, children, hideCloseBtn, sheetOnPhone, size, onOpenAutoFocus, +3 more. Hooks: useRef. Renders: span, DialogPortal, DialogOverlay, DialogPrimitive.Content, DialogPrimitive.Close, X. |
| `apps/web/components/ui/dialog::DialogDescription` | apps/web/components/ui/dialog.tsx | all | component | Wrapped component. Props: className, ...props. Renders: DialogPrimitive.Description. |
| `apps/web/components/ui/dialog::DialogFooter` | apps/web/components/ui/dialog.tsx | all | component | Arrow function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/dialog::DialogHeader` | apps/web/components/ui/dialog.tsx | all | component | Arrow function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/dialog::DialogOverlay` | apps/web/components/ui/dialog.tsx | all | component | Wrapped component. Props: className, ...props. Renders: DialogPrimitive.Overlay. |
| `apps/web/components/ui/dialog::DialogTitle` | apps/web/components/ui/dialog.tsx | all | component | Wrapped component. Props: className, ...props. Renders: DialogPrimitive.Title. |
| `apps/web/components/ui/dropdown-menu::DropdownMenuCheckboxItem` | apps/web/components/ui/dropdown-menu.tsx | all | component | Wrapped component. Props: className, children, checked, ...props. Renders: span, DropdownMenuPrimitive.CheckboxItem, DropdownMenuPrimitive.ItemIndicator, Check. |
| `apps/web/components/ui/dropdown-menu::DropdownMenuContent` | apps/web/components/ui/dropdown-menu.tsx | all | component | Wrapped component. Props: className, sideOffset, collisionPadding, ...props. Renders: DropdownMenuPrimitive.Portal, DropdownMenuPrimitive.Content. |
| `apps/web/components/ui/dropdown-menu::DropdownMenuItem` | apps/web/components/ui/dropdown-menu.tsx | all | component | Wrapped component. Props: className, inset, variant, ...props. Renders: DropdownMenuPrimitive.Item. |
| `apps/web/components/ui/dropdown-menu::DropdownMenuLabel` | apps/web/components/ui/dropdown-menu.tsx | all | component | Wrapped component. Props: className, inset, ...props. Renders: DropdownMenuPrimitive.Label. |
| `apps/web/components/ui/dropdown-menu::DropdownMenuRadioItem` | apps/web/components/ui/dropdown-menu.tsx | all | component | Wrapped component. Props: className, children, ...props. Renders: span, DropdownMenuPrimitive.RadioItem, DropdownMenuPrimitive.ItemIndicator, Circle. |
| `apps/web/components/ui/dropdown-menu::DropdownMenuSeparator` | apps/web/components/ui/dropdown-menu.tsx | all | component | Wrapped component. Props: className, ...props. Renders: DropdownMenuPrimitive.Separator. |
| `apps/web/components/ui/dropdown-menu::DropdownMenuShortcut` | apps/web/components/ui/dropdown-menu.tsx | all | component | Arrow function component. Props: className, ...props. Renders: span. |
| `apps/web/components/ui/dropdown-menu::DropdownMenuSubContent` | apps/web/components/ui/dropdown-menu.tsx | all | component | Wrapped component. Props: className, collisionPadding, ...props. Renders: DropdownMenuPrimitive.SubContent. |
| `apps/web/components/ui/dropdown-menu::DropdownMenuSubTrigger` | apps/web/components/ui/dropdown-menu.tsx | all | component | Wrapped component. Props: className, inset, children, ...props. Renders: DropdownMenuPrimitive.SubTrigger, ChevronRight. |
| `apps/web/components/ui/empty::Empty` | apps/web/components/ui/empty.tsx | all | component | Function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/empty::EmptyContent` | apps/web/components/ui/empty.tsx | all | component | Function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/empty::EmptyDescription` | apps/web/components/ui/empty.tsx | all | component | Function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/empty::EmptyHeader` | apps/web/components/ui/empty.tsx | all | component | Function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/empty::EmptyMedia` | apps/web/components/ui/empty.tsx | all | component | Function component. Props: className, variant, ...props. Renders: div. |
| `apps/web/components/ui/empty::EmptyTitle` | apps/web/components/ui/empty.tsx | all | component | Function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/field::Field` | apps/web/components/ui/field.tsx | all | component | Function component. Props: className, orientation, ...props. Renders: div. |
| `apps/web/components/ui/field::FieldContent` | apps/web/components/ui/field.tsx | all | component | Function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/field::FieldDescription` | apps/web/components/ui/field.tsx | all | component | Function component. Props: className, ...props. Renders: p. |
| `apps/web/components/ui/field::FieldError` | apps/web/components/ui/field.tsx | all | component | Function component. Props: className, children, errors, ...props. Hooks: useMemo. Renders: ul, li, div. |
| `apps/web/components/ui/field::FieldGroup` | apps/web/components/ui/field.tsx | all | component | Function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/field::FieldLabel` | apps/web/components/ui/field.tsx | all | component | Function component. Props: className, ...props. Renders: Label. |
| `apps/web/components/ui/field::FieldLegend` | apps/web/components/ui/field.tsx | all | component | Function component. Props: className, variant, ...props. Renders: legend. |
| `apps/web/components/ui/field::FieldSeparator` | apps/web/components/ui/field.tsx | all | component | Function component. Props: children, className, ...props. Renders: div, span, Separator. |
| `apps/web/components/ui/field::FieldSet` | apps/web/components/ui/field.tsx | all | component | Function component. Props: className, ...props. Renders: fieldset. |
| `apps/web/components/ui/field::FieldTitle` | apps/web/components/ui/field.tsx | all | component | Function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/file-picker-button::FilePickerButton` | apps/web/components/ui/file-picker-button.tsx | all | component | Arrow function component. Props: onFileSelect, accept, multiple, ...buttonProps. Hooks: useRef. Renders: div, input, ActionButton. |
| `apps/web/components/ui/form::FormControl` | apps/web/components/ui/form.tsx | all | component | Wrapped component. Props: ...props. Hooks: useFormField. Renders: Slot. |
| `apps/web/components/ui/form::FormDescription` | apps/web/components/ui/form.tsx | all | component | Wrapped component. Props: className, ...props. Hooks: useFormField. Renders: p. |
| `apps/web/components/ui/form::FormField` | apps/web/components/ui/form.tsx | all | component | Arrow function component. Props: ...props. Renders: FormFieldContext.Provider, Controller. |
| `apps/web/components/ui/form::FormItem` | apps/web/components/ui/form.tsx | all | component | Wrapped component. Props: className, ...props. Hooks: useId. Renders: div, FormItemContext.Provider. |
| `apps/web/components/ui/form::FormLabel` | apps/web/components/ui/form.tsx | all | component | Wrapped component. Props: className, ...props. Hooks: useFormField. Renders: Label. |
| `apps/web/components/ui/form::FormMessage` | apps/web/components/ui/form.tsx | all | component | Wrapped component. Props: className, children, ...props. Hooks: useFormField. Renders: p. |
| `apps/web/components/ui/formatted-date::FormattedDate` | apps/web/components/ui/formatted-date.tsx | all | component | Function component. Props: date, formatStr. Hooks: useTranslation, useState, useEffect. |
| `apps/web/components/ui/full-page-spinner::FullPageSpinner` | apps/web/components/ui/full-page-spinner.tsx | all | component | Function component. Renders: div, Spinner. |
| `apps/web/components/ui/info-tooltip::InfoTooltip` | apps/web/components/ui/info-tooltip.tsx | all | component | Function component. Props: className, children, size, variant. Renders: Tooltip, TooltipTrigger, Info, HelpCircle, TooltipContent. |
| `apps/web/components/ui/input::Input` | apps/web/components/ui/input.tsx | all | component | Wrapped component. Props: className, type, startIcon, endIcon, variant, ...props. Renders: div, input. |
| `apps/web/components/ui/kbd::Kbd` | apps/web/components/ui/kbd.tsx | all | component | Function component. Props: className, ...props. Renders: kbd. |
| `apps/web/components/ui/kbd::KbdGroup` | apps/web/components/ui/kbd.tsx | all | component | Function component. Props: className, ...props. Renders: kbd. |
| `apps/web/components/ui/label::Label` | apps/web/components/ui/label.tsx | all | component | Wrapped component. Props: className, ...props. Renders: LabelPrimitive.Root. |
| `apps/web/components/ui/markdown/markdown-editor::MarkdownEditor` | apps/web/components/ui/markdown/markdown-editor.tsx | all | component | Wrapped component. Props: children, onSave, onCancel, isSaving, onDraftChange. Hooks: useTranslation, useRef, useState, useMemo. Renders: div, LexicalComposer, ToolbarPlugin, PlainTextPlugin, ContentEditable, RichTextPlugin, Button. |
| `apps/web/components/ui/markdown/markdown-readonly::MarkdownReadonly` | apps/web/components/ui/markdown/markdown-readonly.tsx | all | component | Function component. Props: children, className, onSave, skipHtml. Renders: input, code, Markdown, PreWithCopyBtn, SyntaxHighlighter. |
| `apps/web/components/ui/markdown/markdown-readonly::PreWithCopyBtn` | apps/web/components/ui/markdown/markdown-readonly.tsx | all | component | Function component. Props: className, ...props. Hooks: useRef. Renders: span, pre, CopyBtn. |
| `apps/web/components/ui/markdown/plugins/toolbar-plugin::MarkdownToolTip` | apps/web/components/ui/markdown/plugins/toolbar-plugin.tsx | all | component | Function component. Hooks: useTranslation. Renders: table, thead, tr, th, tbody, td, Popover, Tooltip, +4 more. |
| `apps/web/components/ui/markdown/plugins/toolbar-plugin::ToolbarPlugin` | apps/web/components/ui/markdown/plugins/toolbar-plugin.tsx | all | component | Function component. Props: isRawMarkdownMode, setIsRawMarkdownMode. Hooks: useTranslation, useLexicalComposerContext, useState, useCallback, useEffect. Renders: div, ButtonWithTooltip, Icon, Switch, Label, MarkdownToolTip. |
| `apps/web/components/ui/multiple-choice-dialog::MultipleChoiceDialog` | apps/web/components/ui/multiple-choice-dialog.tsx | all | component | Function component. Props: open, setOpen, onOpenChange, title, description, actionButtons, +1 more. Hooks: useState. Renders: Dialog, DialogTrigger, DialogContent, DialogHeader, DialogTitle, DialogFooter. |
| `apps/web/components/ui/page-header::PageHeader` | apps/web/components/ui/page-header.tsx | all | component | Function component. Props: title, description, icon, meta, actions, className. Renders: div, span, h1, p. |
| `apps/web/components/ui/password-input::PasswordInput` | apps/web/components/ui/password-input.tsx | all | component | Wrapped component. Props: className, id, disabled, ...props. Hooks: useTranslation, useState. Renders: div, Input, ButtonWithTooltip, EyeOff, Eye. |
| `apps/web/components/ui/progress::Progress` | apps/web/components/ui/progress.tsx | all | component | Wrapped component. Props: className, value, ...props. Renders: ProgressPrimitive.Root, ProgressPrimitive.Indicator. |
| `apps/web/components/ui/radio-group::RadioGroup` | apps/web/components/ui/radio-group.tsx | all | component | Wrapped component. Props: className, ...props. Renders: RadioGroupPrimitive.Root. |
| `apps/web/components/ui/radio-group::RadioGroupItem` | apps/web/components/ui/radio-group.tsx | all | component | Wrapped component. Props: className, ...props. Renders: RadioGroupPrimitive.Item, RadioGroupPrimitive.Indicator, Circle. |
| `apps/web/components/ui/relative-time::RelativeTime` | apps/web/components/ui/relative-time.tsx | all | component | Function component. Props: date. Hooks: useTranslation, useRelativeTime. Renders: time. |
| `apps/web/components/ui/scroll-area::ScrollArea` | apps/web/components/ui/scroll-area.tsx | all | component | Wrapped component. Props: className, children, ...props. Renders: ScrollAreaPrimitive.Root, ScrollAreaPrimitive.Viewport, ScrollBar, ScrollAreaPrimitive.Corner. |
| `apps/web/components/ui/scroll-area::ScrollBar` | apps/web/components/ui/scroll-area.tsx | all | component | Wrapped component. Props: className, orientation, ...props. Renders: ScrollAreaPrimitive.ScrollAreaScrollbar, ScrollAreaPrimitive.ScrollAreaThumb. |
| `apps/web/components/ui/select::SelectContent` | apps/web/components/ui/select.tsx | all | component | Wrapped component. Props: className, children, position, ...props. Renders: SelectPrimitive.Portal, SelectPrimitive.Content, SelectScrollUpButton, SelectPrimitive.Viewport, SelectScrollDownButton. |
| `apps/web/components/ui/select::SelectItem` | apps/web/components/ui/select.tsx | all | component | Wrapped component. Props: className, children, ...props. Renders: span, SelectPrimitive.Item, SelectPrimitive.ItemIndicator, Check, SelectPrimitive.ItemText. |
| `apps/web/components/ui/select::SelectLabel` | apps/web/components/ui/select.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SelectPrimitive.Label. |
| `apps/web/components/ui/select::SelectScrollDownButton` | apps/web/components/ui/select.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SelectPrimitive.ScrollDownButton, ChevronDown. |
| `apps/web/components/ui/select::SelectScrollUpButton` | apps/web/components/ui/select.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SelectPrimitive.ScrollUpButton, ChevronUp. |
| `apps/web/components/ui/select::SelectSeparator` | apps/web/components/ui/select.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SelectPrimitive.Separator. |
| `apps/web/components/ui/select::SelectTrigger` | apps/web/components/ui/select.tsx | all | component | Wrapped component. Props: className, children, ...props. Renders: SelectPrimitive.Trigger, SelectPrimitive.Icon, ChevronDown. |
| `apps/web/components/ui/separator::Separator` | apps/web/components/ui/separator.tsx | all | component | Wrapped component. Props: className, orientation, decorative, ...props. Renders: SeparatorPrimitive.Root. |
| `apps/web/components/ui/skeleton::Skeleton` | apps/web/components/ui/skeleton.tsx | all | component | Function component. Props: className, ...props. Renders: div. |
| `apps/web/components/ui/slider::Slider` | apps/web/components/ui/slider.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SliderPrimitive.Root, SliderPrimitive.Track, SliderPrimitive.Range, SliderPrimitive.Thumb. |
| `apps/web/components/ui/slider::StepperSlider` | apps/web/components/ui/slider.tsx | all | component | Function component. Props: label, decreaseLabel, increaseLabel, value, displayValue, min, +5 more. Renders: div, span, ButtonWithTooltip, Minus, Slider, Plus. |
| `apps/web/components/ui/sonner::Toaster` | apps/web/components/ui/sonner.tsx | all | component | Arrow function component. Props: ...props. Hooks: useTheme. Renders: Sonner, CircleCheck, Info, TriangleAlert, OctagonX, LoaderCircle. |
| `apps/web/components/ui/spinner::LoadingSpinner` | apps/web/components/ui/spinner.tsx | all | component | Function component. Props: className. Renders: svg, path. |
| `apps/web/components/ui/stat-tile::StatTile` | apps/web/components/ui/stat-tile.tsx | all | component | Function component. Props: label, value, icon, action, helper, loading, +4 more. Renders: div, span, button, Icon, Skeleton, Link. |
| `apps/web/components/ui/switch::Switch` | apps/web/components/ui/switch.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SwitchPrimitives.Root, SwitchPrimitives.Thumb. |
| `apps/web/components/ui/table::StackedLabel` | apps/web/components/ui/table.tsx | all | component | Function component. Props: children. Renders: span. |
| `apps/web/components/ui/table::Table` | apps/web/components/ui/table.tsx | all | component | Wrapped component. Props: className, inCard, ...props. Renders: div, table. |
| `apps/web/components/ui/table::TableBody` | apps/web/components/ui/table.tsx | all | component | Wrapped component. Props: className, ...props. Renders: tbody. |
| `apps/web/components/ui/table::TableCaption` | apps/web/components/ui/table.tsx | all | component | Wrapped component. Props: className, ...props. Renders: caption. |
| `apps/web/components/ui/table::TableCell` | apps/web/components/ui/table.tsx | all | component | Wrapped component. Props: className, ...props. Renders: td. |
| `apps/web/components/ui/table::TableFooter` | apps/web/components/ui/table.tsx | all | component | Wrapped component. Props: className, ...props. Renders: tfoot. |
| `apps/web/components/ui/table::TableHead` | apps/web/components/ui/table.tsx | all | component | Wrapped component. Props: className, ...props. Renders: th. |
| `apps/web/components/ui/table::TableHeader` | apps/web/components/ui/table.tsx | all | component | Wrapped component. Props: className, ...props. Renders: thead. |
| `apps/web/components/ui/table::TableRow` | apps/web/components/ui/table.tsx | all | component | Wrapped component. Props: className, ...props. Renders: tr. |
| `apps/web/components/ui/tabs::TabsContent` | apps/web/components/ui/tabs.tsx | all | component | Wrapped component. Props: className, ...props. Renders: TabsPrimitive.Content. |
| `apps/web/components/ui/tabs::TabsList` | apps/web/components/ui/tabs.tsx | all | component | Wrapped component. Props: className, ...props. Renders: TabsPrimitive.List. |
| `apps/web/components/ui/tabs::TabsTrigger` | apps/web/components/ui/tabs.tsx | all | component | Wrapped component. Props: className, ...props. Renders: TabsPrimitive.Trigger. |
| `apps/web/components/ui/textarea::Textarea` | apps/web/components/ui/textarea.tsx | all | component | Wrapped component. Props: className, ...props. Renders: SharedTextarea. |
| `apps/web/components/ui/toast::Toast` | apps/web/components/ui/toast.tsx | all | component | Wrapped component. Props: className, variant, ...props. Renders: ToastPrimitives.Root. |
| `apps/web/components/ui/toast::ToastAction` | apps/web/components/ui/toast.tsx | all | component | Wrapped component. Props: className, ...props. Renders: ToastPrimitives.Action. |
| `apps/web/components/ui/toast::ToastClose` | apps/web/components/ui/toast.tsx | all | component | Wrapped component. Props: className, ...props. Renders: ToastPrimitives.Close, X. |
| `apps/web/components/ui/toast::ToastDescription` | apps/web/components/ui/toast.tsx | all | component | Wrapped component. Props: className, ...props. Renders: ToastPrimitives.Description. |
| `apps/web/components/ui/toast::ToastTitle` | apps/web/components/ui/toast.tsx | all | component | Wrapped component. Props: className, ...props. Renders: ToastPrimitives.Title. |
| `apps/web/components/ui/toast::ToastViewport` | apps/web/components/ui/toast.tsx | all | component | Wrapped component. Props: className, ...props. Renders: ToastPrimitives.Viewport. |
| `apps/web/components/ui/toggle::Toggle` | apps/web/components/ui/toggle.tsx | all | component | Wrapped component. Props: className, variant, size, ...props. Renders: TogglePrimitive.Root. |
| `apps/web/components/ui/tooltip::TooltipContent` | apps/web/components/ui/tooltip.tsx | all | component | Wrapped component. Props: className, sideOffset, children, ...props. Renders: TooltipPrimitive.Content, TooltipPrimitive.Arrow. |
| `apps/web/components/ui/tooltip::TooltipTrigger` | apps/web/components/ui/tooltip.tsx | all | component | Wrapped component. Props: onFocus, onPointerMove, ...props. Renders: TooltipPrimitive.Trigger. |
| `apps/web/components/ui/user-avatar::UserAvatar` | apps/web/components/ui/user-avatar.tsx | all | component | Function component. Props: image, name, className, imgClassName, fallbackClassName, fallback. Hooks: useMemo. Renders: Avatar, AvatarImage, AvatarFallback. |
| `apps/web/components/utils/BookmarkSavedToast::BookmarkSavedToast` | apps/web/components/utils/BookmarkSavedToast.tsx | all | component | Function component. Props: bookmarkId. Renders: div, Link, ExternalLink. |
| `apps/web/components/utils/ValidAccountCheck::ValidAccountCheck` | apps/web/components/utils/ValidAccountCheck.tsx | all | component | Function component. Hooks: useTRPC, useRouter, useQuery, useEffect. |
| `apps/web/components/wrapped/ShareButton::ShareButton` | apps/web/components/wrapped/ShareButton.tsx | all | component | Function component. Props: contentRef, fileName. Hooks: useState. Renders: Button, Loader2, Share2, Download. |
| `apps/web/components/wrapped/WrappedContent::WrappedContent` | apps/web/components/wrapped/WrappedContent.tsx | all | component | Wrapped component. Props: stats, userName. Renders: div, h1, p, h2, h3, span, Card, Calendar, +4 more. |
| `apps/web/components/wrapped/WrappedModal::WrappedModal` | apps/web/components/wrapped/WrappedModal.tsx | all | component | Function component. Props: open, onClose. Hooks: useTRPC, useRef, useQuery. Renders: div, button, p, Dialog, DialogOverlay, DialogContent, VisuallyHidden.Root, DialogTitle, +1 more. |
| `apps/web/lib/i18n/provider::CustomI18nextProvider` | apps/web/lib/i18n/provider.tsx | all | component | Arrow function component. Props: lang, children. Renders: I18nextProvider. |
| `apps/web/lib/providers::Providers` | apps/web/lib/providers.tsx | all | component | Function component. Props: children, session, clientConfig, userLocalSettings. Hooks: useEffect, useState. Renders: ClientConfigProvider, UserLocalSettingsCtx.Provider, SessionProvider, QueryClientProvider, TRPCProvider, CustomI18nextProvider. |
| `apps/web/lib/readerSettings::ReaderSettingsProvider` | apps/web/lib/readerSettings.tsx | all | component | Function component. Props: children. Hooks: useState, useMemo, useCallback. Renders: BaseReaderSettingsProvider, SessionOverridesContext.Provider. |
| `apps/web/lib/userSettings::UserSettingsContextProvider` | apps/web/lib/userSettings.tsx | all | component | Function component. Props: userSettings, children. Hooks: useTRPC, useQuery. Renders: UserSettingsContext.Provider. |
| `docs/src/theme/DocSidebarItem/Category/index::CollapseButton` | docs/src/theme/DocSidebarItem/Category/index.tsx | all | component | Function component. Props: collapsed, categoryLabel, onClick. Renders: button. |
| `docs/src/theme/DocSidebarItem/Category/index::DocSidebarItemCategory` | docs/src/theme/DocSidebarItem/Category/index.tsx | all | component | Function component. Props: item, onItemClick, activePath, level, index, ...props. Hooks: useThemeConfig, useCategoryHrefWithSSRFallback, useCollapsible, useDocSidebarItemsExpandedState, useAutoExpandActiveCategory, useEffect. Renders: li, div, span, Link, Icon, CollapseButton, Collapsible, DocSidebarItems. |
| `packages/benchmarks/setup/html/hello.html::PackagesBenchmarksSetupHtmlHelloPage` | packages/benchmarks/setup/html/hello.html | all | component | Web page at /packages/benchmarks/setup/html/hello, titled "Benchmarks Fixture". 0 interactive elements. |
| `packages/e2e_tests/setup/html/article.html::PackagesE2eTestsSetupHtmlArticlePage` | packages/e2e_tests/setup/html/article.html | all | component | Web page at /packages/e2e_tests/setup/html/article, titled "Article title". 0 interactive elements. |
| `packages/e2e_tests/setup/html/hello.html::PackagesE2eTestsSetupHtmlHelloPage` | packages/e2e_tests/setup/html/hello.html | all | component | Web page at /packages/e2e_tests/setup/html/hello, titled "My test title". 0 interactive elements. |
| `packages/shared-react/components/BookmarkHtmlHighlighter::BookmarkHTMLHighlighter` | packages/shared-react/components/BookmarkHtmlHighlighter.tsx | all | component | Wrapped component. Props: htmlContent, className, style, highlights, readOnly, onHighlight, +4 more. Hooks: useRef, useImperativeHandle, useState, useEffect, useMemo. Renders: div, HighlightDock, HighlightForm. |
| `packages/shared-react/components/BookmarkHtmlHighlighter::HighlightDock` | packages/shared-react/components/BookmarkHtmlHighlighter.tsx | all | component | Arrow function component. Props: open, bottomOffset, saving, labels, selectedHighlight, onClose, +3 more. Hooks: useState, useRef, useEffect. Renders: div, p, button, Check, Trash2, X, Textarea. |
| `packages/shared-react/components/BookmarkHtmlHighlighter::HighlightForm` | packages/shared-react/components/BookmarkHtmlHighlighter.tsx | all | component | Arrow function component. Props: position, selectedHighlight, onClose, onSave, onDelete, isMobile. Hooks: useState, useEffect, useMemo. Renders: div, label, Popover, PopoverAnchor, PopoverContent, Button, Check, Textarea. |
| `packages/shared-react/components/ScrollProgressTracker::ScrollProgressTracker` | packages/shared-react/components/ScrollProgressTracker.tsx | all | component | Wrapped component. Props: onSavePosition, onScrollPositionChange, restorePosition, readingProgressOffset, readingProgressAnchor, showProgressBar, +5 more. Hooks: useRef, useImperativeHandle, useState, useEffect. Renders: div. |
| `packages/shared-react/components/ui/button::Button` | packages/shared-react/components/ui/button.tsx | all | component | Wrapped component. Props: className, variant, size, asChild, ...props. Renders: Comp. |
| `packages/shared-react/components/ui/popover::PopoverContent` | packages/shared-react/components/ui/popover.tsx | all | component | Wrapped component. Props: className, align, sideOffset, ...props. Renders: PopoverPrimitive.Portal, PopoverPrimitive.Content. |
| `packages/shared-react/components/ui/textarea::Textarea` | packages/shared-react/components/ui/textarea.tsx | all | component | Wrapped component. Props: className, ...props. Renders: textarea. |
| `packages/shared-react/hooks/bookmark-grid-context::BookmarkGridContextProvider` | packages/shared-react/hooks/bookmark-grid-context.tsx | all | component | Function component. Props: query, children. Renders: BookmarkGridContext.Provider. |
| `packages/shared-react/hooks/bookmark-list-context::BookmarkListContextProvider` | packages/shared-react/hooks/bookmark-list-context.tsx | all | component | Function component. Props: list, children. Renders: BookmarkListContext.Provider. |
| `packages/shared-react/hooks/reader-settings::ReaderSettingsProvider` | packages/shared-react/hooks/reader-settings.tsx | all | component | Function component. Props: children, ...options. Hooks: useReaderSettings. Renders: ReaderSettingsContext.Provider. |
| `packages/shared-react/providers/client-config-provider::ClientConfigProvider` | packages/shared-react/providers/client-config-provider.tsx | all | component | Function component. Props: children, value. Hooks: useMemo. Renders: ClientConfigContext.Provider. |
| `packages/shared-react/providers/trpc-provider::TRPCSettingsProvider` | packages/shared-react/providers/trpc-provider.tsx | all | component | Function component. Props: settings, queryClient, children. Hooks: useMemo. Renders: QueryClientProvider, TRPCProvider. |

## Coverage

- all: 803 identifier(s)

## Design system components

803 component(s) carry a stable `@uxid`. 41 declare variants (50 axis/axes, 164 value(s) in total), read from `cva()` calls, class maps, prop unions and conditional class branches.

131 of them are primitives under `apps/web/components/ui`, identified by a `apps/web/components/ui` directory of 47 files. 678 are application components, of which 205 are rendered in exactly one other file and 291 are rendered nowhere else (a page, or dead code).

| @uxid | component | file | variants | states | uses | notes |
| --- | --- | --- | --- | --- | --- | --- |
| "apps/browser-extension/src/BookmarkDeletedPage::BookmarkDeletedPage" | BookmarkDeletedPage | `apps/browser-extension/src/BookmarkDeletedPage.tsx` |  |  | 1 | Confirmation screen shown in the extension after a bookmark has been deleted. |
| "apps/browser-extension/src/BookmarkSavedPage::Section" | Section | `apps/browser-extension/src/BookmarkSavedPage.tsx` |  | active, dark, hover | 3 | Labelled grouping block used to organise content on the saved-bookmark screen. |
| "apps/browser-extension/src/BookmarkSavedPage::BookmarkSavedPage" | BookmarkSavedPage | `apps/browser-extension/src/BookmarkSavedPage.tsx` |  | active, dark, hover | 1 | Screen shown after a page has been bookmarked, where the saved bookmark can be reviewed and edited. |
| "apps/browser-extension/src/Layout::Layout" | Layout | `apps/browser-extension/src/Layout.tsx` |  | hover | 2 | Outer shell that frames every screen of the extension popup. |
| "apps/browser-extension/src/Logo::Logo" | Logo | `apps/browser-extension/src/Logo.tsx` |  | dark | 3 | Product logo mark rendered inside the extension. |
| "apps/browser-extension/src/OptionsPage::OptionsPage" | OptionsPage | `apps/browser-extension/src/OptionsPage.tsx` |  | dark, focus, hover | 1 | Extension options/settings screen. |
| "apps/browser-extension/src/OptionsPage::SettingsSection" | SettingsSection | `apps/browser-extension/src/OptionsPage.tsx` |  | dark, focus, hover | 31 | Titled group of related settings on the options screen. |
| "apps/browser-extension/src/OptionsPage::SettingsRow" | SettingsRow | `apps/browser-extension/src/OptionsPage.tsx` |  | dark, focus, hover | 20 | Single setting row pairing a label with its control on the options screen. |
| "apps/browser-extension/src/SavePage::SavePage" | SavePage | `apps/browser-extension/src/SavePage.tsx` |  | active | 1 | Screen that saves the current browser page as a bookmark. |
| "apps/browser-extension/src/ServerAddressPage::ServerAddressPage" | ServerAddressPage | `apps/browser-extension/src/ServerAddressPage.tsx` |  | hover | 1 | Screen for entering the address of the server the extension connects to. |
| "apps/browser-extension/src/SignInPage::SignInPage" | SignInPage | `apps/browser-extension/src/SignInPage.tsx` |  | hover | 1 | Authentication screen for signing the user into their account. |
| "apps/browser-extension/src/Spinner::Spinner" | Spinner | `apps/browser-extension/src/Spinner.tsx` |  |  | 10 | Loading indicator used while the extension waits on an operation. |
| "apps/browser-extension/src/components/BookmarkLists::ListPathLabel" | ListPathLabel | `apps/browser-extension/src/components/BookmarkLists.tsx` |  | hover | 1 | Displays the hierarchical path of a bookmark list as a label. |
| "apps/browser-extension/src/components/BookmarkLists::BookmarkLists" | BookmarkLists | `apps/browser-extension/src/components/BookmarkLists.tsx` |  | hover | 1 | Shows the lists a bookmark belongs to. |
| "apps/browser-extension/src/components/ErrorCallout::ErrorCallout" | ErrorCallout | `apps/browser-extension/src/components/ErrorCallout.tsx` |  |  | 6 | Inline callout surfacing an error message to the user. |
| "apps/browser-extension/src/components/ListsSelector::ListsSelector" | ListsSelector | `apps/browser-extension/src/components/ListsSelector.tsx` |  | hover | 1 | Picker for adding a bookmark to one or more lists. |
| "apps/browser-extension/src/components/NoteEditor::NoteEditor" | NoteEditor | `apps/browser-extension/src/components/NoteEditor.tsx` |  | dark | 2 | Editable field for attaching or changing a note on a bookmark. |
| "apps/browser-extension/src/components/PopupHeader::PopupHeader" | PopupHeader | `apps/browser-extension/src/components/PopupHeader.tsx` |  | hover | 3 | Header bar at the top of the extension popup. |
| "apps/browser-extension/src/components/PopupHeader::HeaderIconButton" | HeaderIconButton | `apps/browser-extension/src/components/PopupHeader.tsx` |  | hover | 3 | Icon-only action button placed in the popup header. |
| "apps/browser-extension/src/components/StatusMessage::StatusMessage" | StatusMessage | `apps/browser-extension/src/components/StatusMessage.tsx` |  |  | 3 | Short status text reporting the outcome or progress of an action. |
| "apps/browser-extension/src/components/TagList::TagList" | TagList | `apps/browser-extension/src/components/TagList.tsx` |  | dark | 7 | Displays the tags attached to a bookmark. |
| "apps/browser-extension/src/components/TagsSelector::TagsSelector" | TagsSelector | `apps/browser-extension/src/components/TagsSelector.tsx` |  | hover | 1 | Picker for adding or removing tags on a bookmark. |
| "apps/browser-extension/src/components/TitleEditor::TitleEditor" | TitleEditor | `apps/browser-extension/src/components/TitleEditor.tsx` |  |  | 2 | Editable field for changing a bookmark's title. |
| "apps/browser-extension/src/components/ui/badge::Badge" | Badge | `apps/browser-extension/src/components/ui/badge.tsx` | variant (4) | focus, hover | 52 | Small label chip primitive, used for compact status or tag-like markers. |
| "apps/browser-extension/src/components/ui/button::Button" | Button | `apps/browser-extension/src/components/ui/button.tsx` | variant (6), size (4) | dark, disabled, focus-visible, hover | 205 | Base button primitive for actions throughout the extension. |
| "apps/browser-extension/src/components/ui/command::Command" | Command | `apps/browser-extension/src/components/ui/command.tsx` |  | aria-selected, disabled, placeholder | 13 | Root of the searchable command/selection palette primitive. |
| "apps/browser-extension/src/components/ui/command::CommandDialog" | CommandDialog | `apps/browser-extension/src/components/ui/command.tsx` |  | aria-selected, disabled, placeholder | 0 | Command palette presented inside a dialog. |
| "apps/browser-extension/src/components/ui/command::CommandInput" | CommandInput | `apps/browser-extension/src/components/ui/command.tsx` |  | aria-selected, disabled, placeholder | 10 | Search/filter input at the top of the command palette. |
| "apps/browser-extension/src/components/ui/command::CommandList" | CommandList | `apps/browser-extension/src/components/ui/command.tsx` |  | aria-selected, disabled, placeholder | 11 | Scrollable list container for command palette results. |
| "apps/browser-extension/src/components/ui/command::CommandEmpty" | CommandEmpty | `apps/browser-extension/src/components/ui/command.tsx` |  | aria-selected, disabled, placeholder | 10 | Empty-state message shown when the command palette has no matches. |
| "apps/browser-extension/src/components/ui/command::CommandGroup" | CommandGroup | `apps/browser-extension/src/components/ui/command.tsx` |  | aria-selected, disabled, placeholder | 12 | Headed group of related items within the command palette. |
| "apps/browser-extension/src/components/ui/command::CommandSeparator" | CommandSeparator | `apps/browser-extension/src/components/ui/command.tsx` |  | aria-selected, disabled, placeholder | 1 | Divider between groups in the command palette. |
| "apps/browser-extension/src/components/ui/command::CommandItem" | CommandItem | `apps/browser-extension/src/components/ui/command.tsx` |  | aria-selected, disabled, placeholder | 15 | Individual selectable row in the command palette. |
| "apps/browser-extension/src/components/ui/command::CommandShortcut" | CommandShortcut | `apps/browser-extension/src/components/ui/command.tsx` |  | aria-selected, disabled, placeholder | 0 | Right-aligned keyboard shortcut hint on a command item. |
| "apps/browser-extension/src/components/ui/dialog::DialogOverlay" | DialogOverlay | `apps/browser-extension/src/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus, hover | 2 | Backdrop layer rendered behind an open dialog. |
| "apps/browser-extension/src/components/ui/dialog::DialogContent" | DialogContent | `apps/browser-extension/src/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus, hover | 36 | Main panel of a modal dialog. |
| "apps/browser-extension/src/components/ui/dialog::DialogHeader" | DialogHeader | `apps/browser-extension/src/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus, hover | 31 | Top region of a dialog holding its title and description. |
| "apps/browser-extension/src/components/ui/dialog::DialogFooter" | DialogFooter | `apps/browser-extension/src/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus, hover | 24 | Bottom region of a dialog holding its action buttons. |
| "apps/browser-extension/src/components/ui/dialog::DialogTitle" | DialogTitle | `apps/browser-extension/src/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus, hover | 35 | Heading text of a dialog. |
| "apps/browser-extension/src/components/ui/dialog::DialogDescription" | DialogDescription | `apps/browser-extension/src/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus, hover | 13 | Supporting description text beneath a dialog title. |
| "apps/browser-extension/src/components/ui/dynamic-popover::DynamicPopoverContent" | DynamicPopoverContent | `apps/browser-extension/src/components/ui/dynamic-popover.tsx` |  | data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed], data-[state=open] | 2 | Popover content variant for the browser extension that adapts its positioning or sizing dynamically, used for floating panels anchored to a trigger. |
| "apps/browser-extension/src/components/ui/input::Input" | Input | `apps/browser-extension/src/components/ui/input.tsx` |  | dark, disabled, file, focus-visible, placeholder | 80 | Single-line text input primitive for extension forms, styled against the shared input, ring and border tokens. |
| "apps/browser-extension/src/components/ui/popover::PopoverContent" | PopoverContent | `apps/browser-extension/src/components/ui/popover.tsx` |  | data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed], data-[state=open] | 17 | Standard floating popover surface in the extension, using the popover and popover-foreground tokens for its panel. |
| "apps/browser-extension/src/components/ui/select::SelectTrigger" | SelectTrigger | `apps/browser-extension/src/components/ui/select.tsx` |  | data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed] | 29 | Clickable control that opens a select dropdown and displays the current value. |
| "apps/browser-extension/src/components/ui/select::SelectScrollUpButton" | SelectScrollUpButton | `apps/browser-extension/src/components/ui/select.tsx` |  | data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed] | 1 | Scroll affordance shown at the top of a long select list to scroll options upward. |
| "apps/browser-extension/src/components/ui/select::SelectScrollDownButton" | SelectScrollDownButton | `apps/browser-extension/src/components/ui/select.tsx` |  | data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed] | 1 | Scroll affordance shown at the bottom of a long select list to scroll options downward. |
| "apps/browser-extension/src/components/ui/select::SelectContent" | SelectContent | `apps/browser-extension/src/components/ui/select.tsx` |  | data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed] | 29 | Floating listbox panel that contains the select's options, labels and separators. |
| "apps/browser-extension/src/components/ui/select::SelectLabel" | SelectLabel | `apps/browser-extension/src/components/ui/select.tsx` |  | data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed] | 0 | Non-interactive heading used to title a group of options inside a select list. |
| "apps/browser-extension/src/components/ui/select::SelectItem" | SelectItem | `apps/browser-extension/src/components/ui/select.tsx` |  | data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed] | 82 | Individual selectable option row within the select list, with hover and selected states. |
| "apps/browser-extension/src/components/ui/select::SelectSeparator" | SelectSeparator | `apps/browser-extension/src/components/ui/select.tsx` |  | data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed] | 0 | Thin divider used to visually separate option groups inside a select list. |
| "apps/browser-extension/src/components/ui/switch::Switch" | Switch | `apps/browser-extension/src/components/ui/switch.tsx` |  | dark, data-[state=checked], data-[state=unchecked], disabled, focus-visible | 26 | Binary on/off toggle control for extension settings. |
| "apps/browser-extension/src/components/ui/textarea::Textarea" | Textarea | `apps/browser-extension/src/components/ui/textarea.tsx` |  | dark, disabled, focus-visible, placeholder | 12 | Multi-line text input for longer free-form entry in the extension. |
| "apps/browser-extension/src/main::App" | App | `apps/browser-extension/src/main.tsx` |  |  | 0 | Root component of the browser extension that mounts the UI tree. |
| "apps/browser-extension/src/utils/ThemeProvider::ThemeProvider" | ThemeProvider | `apps/browser-extension/src/utils/ThemeProvider.tsx` | currentTheme (2) |  | 2 | Context provider that applies the active theme (light/dark token set) to the extension. |
| "apps/browser-extension/src/utils/providers::Providers" | Providers | `apps/browser-extension/src/utils/providers.tsx` |  |  | 4 | Composition wrapper that stacks the extension's context providers, including theming, around the app. |
| "apps/landing/components/ui/button::Button" | Button | `apps/landing/components/ui/button.tsx` | variant (7), size (4) | disabled, focus-visible, hover | 205 | Primary call-to-action and action button for the landing site, driven by the primary/secondary semantic color tokens. |
| "apps/landing/src/Apps::ListingSection" | ListingSection | `apps/landing/src/Apps.tsx` |  | hover | 0 | Section block that lists a group of available apps or downloads on the Apps page. |
| "apps/landing/src/Apps::Apps" | Apps | `apps/landing/src/Apps.tsx` |  | hover | 0 | Landing page listing the product's available applications across platforms. |
| "apps/landing/src/Homepage::Homepage" | Homepage | `apps/landing/src/Homepage.tsx` |  |  | 0 | Top-level marketing homepage that assembles the hero, feature showcases, use cases and closing CTA. |
| "apps/landing/src/Navbar::NavBar" | NavBar | `apps/landing/src/Navbar.tsx` |  | hover | 0 | Site-wide navigation bar for the landing site linking to its main pages. |
| "apps/landing/src/Pricing::PricingHeader" | PricingHeader | `apps/landing/src/Pricing.tsx` |  | hover | 0 | Heading area introducing the pricing page. |
| "apps/landing/src/Pricing::PricingCard" | PricingCard | `apps/landing/src/Pricing.tsx` |  | hover | 0 | Card presenting one pricing tier with its details and action. |
| "apps/landing/src/Pricing::CorporateBand" | CorporateBand | `apps/landing/src/Pricing.tsx` |  | hover | 0 | Banner strip on the pricing page addressing corporate or team customers. |
| "apps/landing/src/Pricing::FAQ" | FAQ | `apps/landing/src/Pricing.tsx` |  |  | 0 | Frequently-asked-questions block on the pricing page. |
| "apps/landing/src/Pricing::Pricing" | Pricing | `apps/landing/src/Pricing.tsx` |  | hover | 0 | Pricing page composed of the header, tier cards, corporate band and FAQ. |
| "apps/landing/src/Privacy::PrivacyPolicy" | PrivacyPolicy | `apps/landing/src/Privacy.tsx` |  | hover | 0 | Long-form legal page presenting the privacy policy. |
| "apps/landing/src/Terms::Terms" | Terms | `apps/landing/src/Terms.tsx` |  | hover | 0 | Long-form legal page presenting the terms of service. |
| "apps/landing/src/components/ClosingCta::ClosingCta" | ClosingCta | `apps/landing/src/components/ClosingCta.tsx` |  |  | 1 | Final call-to-action section placed near the end of marketing pages. |
| "apps/landing/src/components/FeatureShowcase::FeatureShowcase" | FeatureShowcase | `apps/landing/src/components/FeatureShowcase.tsx` | tints (4) |  | 5 | Full-width section that pairs feature copy with a visual mockup. |
| "apps/landing/src/components/FeatureShowcase::FeatureShowcaseHalf" | FeatureShowcaseHalf | `apps/landing/src/components/FeatureShowcase.tsx` |  |  | 2 | Half-width variant of the feature showcase for side-by-side feature pairs. |
| "apps/landing/src/components/Footer::Footer" | Footer | `apps/landing/src/components/Footer.tsx` |  | hover | 0 | Site footer with secondary links and legal references. |
| "apps/landing/src/components/LlmReady::LlmReady" | LlmReady | `apps/landing/src/components/LlmReady.tsx` |  |  | 1 | Marketing section highlighting the product's LLM-ready capabilities. |
| "apps/landing/src/components/OpenSource::OpenSource" | OpenSource | `apps/landing/src/components/OpenSource.tsx` |  | hover | 1 | Marketing section highlighting that the product is open source. |
| "apps/landing/src/components/Platforms::Platforms" | Platforms | `apps/landing/src/components/Platforms.tsx` |  | group-hover, hover | 1 | Section showing the platforms on which the product is available. |
| "apps/landing/src/components/TerminalCard::TerminalCard" | TerminalCard | `apps/landing/src/components/TerminalCard.tsx` |  |  | 2 | Card styled like a terminal window, using the monospace typography, for showing commands or code. |
| "apps/landing/src/components/UseCases::SearchModesIcon" | SearchModesIcon | `apps/landing/src/components/UseCases.tsx` |  |  | 0 | Icon illustrating the search modes use case within the use-cases section. |
| "apps/landing/src/components/UseCases::UseCases" | UseCases | `apps/landing/src/components/UseCases.tsx` |  |  | 1 | Section presenting the product's main use cases with accompanying icons. |
| "apps/landing/src/components/showcase/CollabListCardMockup::CollabListCardMockup" | CollabListCardMockup | `apps/landing/src/components/showcase/CollabListCardMockup.tsx` |  |  | 1 | Illustrative mockup of a collaborative list card used inside feature showcases. |
| "apps/landing/src/components/showcase/MockupCard::MockupCard" | MockupCard | `apps/landing/src/components/showcase/MockupCard.tsx` |  |  | 5 | Generic window-style frame for product mockups in showcase sections. |
| "apps/landing/src/components/showcase/MockupCard::TrafficDots" | TrafficDots | `apps/landing/src/components/showcase/MockupCard.tsx` |  |  | 1 | Decorative window-control dots rendered in the header of a mockup card. |
| "apps/landing/src/components/showcase/RssFeedsCardMockup::Toggle" | Toggle | `apps/landing/src/components/showcase/RssFeedsCardMockup.tsx` |  |  | 2 | Small on/off switch used inside the RSS feeds showcase mockup to depict enabling or disabling a feed. |
| "apps/landing/src/components/showcase/RssFeedsCardMockup::RssFeedsCardMockup" | RssFeedsCardMockup | `apps/landing/src/components/showcase/RssFeedsCardMockup.tsx` |  |  | 1 | Landing-page showcase card that illustrates the RSS feed subscription feature as a static mockup. |
| "apps/landing/src/components/showcase/RuleCardMockup::StepLabel" | StepLabel | `apps/landing/src/components/showcase/RuleCardMockup.tsx` |  |  | 0 | Caption label for a single step within the rule automation mockup. |
| "apps/landing/src/components/showcase/RuleCardMockup::StepRow" | StepRow | `apps/landing/src/components/showcase/RuleCardMockup.tsx` |  |  | 0 | One row of the rule mockup representing a trigger, condition or action step. |
| "apps/landing/src/components/showcase/RuleCardMockup::StepConnector" | StepConnector | `apps/landing/src/components/showcase/RuleCardMockup.tsx` |  |  | 0 | Visual connector drawn between consecutive step rows in the rule mockup. |
| "apps/landing/src/components/showcase/RuleCardMockup::RuleCardMockup" | RuleCardMockup | `apps/landing/src/components/showcase/RuleCardMockup.tsx` |  |  | 1 | Landing-page showcase card illustrating the automation rules feature as a sequence of steps. |
| "apps/landing/src/components/showcase/ScreenshotCard::BrowserScreenshotCard" | BrowserScreenshotCard | `apps/landing/src/components/showcase/ScreenshotCard.tsx` |  |  | 1 | Showcase frame that presents a product screenshot inside a browser-window chrome. |
| "apps/landing/src/components/showcase/ScreenshotCard::PaperScreenshotCard" | PaperScreenshotCard | `apps/landing/src/components/showcase/ScreenshotCard.tsx` |  |  | 1 | Showcase frame that presents a screenshot on a flat paper-style card. |
| "apps/landing/src/components/showcase/SearchCardMockup::SearchCardMockup" | SearchCardMockup | `apps/landing/src/components/showcase/SearchCardMockup.tsx` |  |  | 1 | Landing-page showcase card illustrating the search feature as a static mockup. |
| "apps/landing/src/components/showcase/TagsCardMockup::TagChip" | TagChip | `apps/landing/src/components/showcase/TagsCardMockup.tsx` |  |  | 0 | Pill-shaped chip representing a single tag inside the tags showcase mockup. |
| "apps/landing/src/components/showcase/TagsCardMockup::TagsCardMockup" | TagsCardMockup | `apps/landing/src/components/showcase/TagsCardMockup.tsx` |  |  | 1 | Landing-page showcase card illustrating the tagging feature using a set of tag chips. |
| "apps/mobile/app/+not-found::NotFound" | NotFound | `apps/mobile/app/+not-found.tsx` |  |  | 1 | Fallback screen shown in the mobile app when a route cannot be matched. |
| "apps/mobile/app/dashboard/(tabs)/(highlights)/_layout::Layout" | Layout | `apps/mobile/app/dashboard/(tabs)/(highlights)/_layout.tsx` |  |  | 2 | Navigation stack layout for the highlights tab. |
| "apps/mobile/app/dashboard/(tabs)/(highlights)/index::Highlights" | Highlights | `apps/mobile/app/dashboard/(tabs)/(highlights)/index.tsx` |  |  | 0 | Tab screen listing the user's highlights across bookmarks. |
| "apps/mobile/app/dashboard/(tabs)/(home)/_layout::Layout" | Layout | `apps/mobile/app/dashboard/(tabs)/(home)/_layout.tsx` |  |  | 2 | Navigation stack layout for the home tab. |
| "apps/mobile/app/dashboard/(tabs)/(home)/index::Home" | Home | `apps/mobile/app/dashboard/(tabs)/(home)/index.tsx` |  |  | 5 | Primary tab screen showing the user's bookmarks. |
| "apps/mobile/app/dashboard/(tabs)/(lists)/_layout::Layout" | Layout | `apps/mobile/app/dashboard/(tabs)/(lists)/_layout.tsx` |  |  | 2 | Navigation stack layout for the lists tab. |
| "apps/mobile/app/dashboard/(tabs)/(lists)/index::ListRow" | ListRow | `apps/mobile/app/dashboard/(tabs)/(lists)/index.tsx` |  | active, dark | 0 | Single row representing one list in the lists tab. |
| "apps/mobile/app/dashboard/(tabs)/(lists)/index::Lists" | Lists | `apps/mobile/app/dashboard/(tabs)/(lists)/index.tsx` |  | active, dark | 0 | Tab screen enumerating the user's lists via @apps/mobile/app/dashboard/(tabs)/(lists)/index::ListRow. |
| "apps/mobile/app/dashboard/(tabs)/(search)/_layout::Layout" | Layout | `apps/mobile/app/dashboard/(tabs)/(search)/_layout.tsx` |  |  | 2 | Navigation stack layout for the search tab. |
| "apps/mobile/app/dashboard/(tabs)/(search)/index.ios::SearchTab" | SearchTab | `apps/mobile/app/dashboard/(tabs)/(search)/index.ios.tsx` |  | placeholder | 0 | iOS-specific search tab screen for querying bookmarks. |
| "apps/mobile/app/dashboard/(tabs)/(tags)/_layout::Layout" | Layout | `apps/mobile/app/dashboard/(tabs)/(tags)/_layout.tsx` |  |  | 2 | Navigation stack layout for the tags tab. |
| "apps/mobile/app/dashboard/(tabs)/(tags)/index::Tags" | Tags | `apps/mobile/app/dashboard/(tabs)/(tags)/index.tsx` |  | active | 2 | Tab screen listing the user's tags. |
| "apps/mobile/app/dashboard/(tabs)/_layout::TabLayout" | TabLayout | `apps/mobile/app/dashboard/(tabs)/_layout.tsx` |  |  | 0 | Bottom tab navigator that hosts the home, highlights, lists, search and tags tabs. |
| "apps/mobile/app/dashboard/(tabs)/index::TabIndex" | TabIndex | `apps/mobile/app/dashboard/(tabs)/index.tsx` |  |  | 0 | Entry route for the tab group that resolves to the default tab. |
| "apps/mobile/app/dashboard/_layout::Dashboard" | Dashboard | `apps/mobile/app/dashboard/_layout.tsx` |  |  | 0 | Root layout for the authenticated dashboard area of the mobile app. |
| "apps/mobile/app/dashboard/archive::Archive" | Archive | `apps/mobile/app/dashboard/archive.tsx` |  |  | 11 | Screen showing archived bookmarks. |
| "apps/mobile/app/dashboard/bookmarks/[slug]/highlights::BookmarkHighlightsPage" | BookmarkHighlightsPage | `apps/mobile/app/dashboard/bookmarks/[slug]/highlights.tsx` |  |  | 0 | Screen listing the highlights belonging to a single bookmark. |
| "apps/mobile/app/dashboard/bookmarks/[slug]/index::SymbolOrAa" | SymbolOrAa | `apps/mobile/app/dashboard/bookmarks/[slug]/index.tsx` |  |  | 0 | Header control that renders either a symbol icon or a text-size (Aa) affordance for the bookmark reader. |
| "apps/mobile/app/dashboard/bookmarks/[slug]/index::BookmarkView" | BookmarkView | `apps/mobile/app/dashboard/bookmarks/[slug]/index.tsx` |  |  | 0 | Reader screen that displays a single bookmark's content. |
| "apps/mobile/app/dashboard/bookmarks/[slug]/info::TitleEditor" | TitleEditor | `apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx` |  | active | 1 | Inline editor for changing a bookmark's title on the info screen. |
| "apps/mobile/app/dashboard/bookmarks/[slug]/info::NotesEditor" | NotesEditor | `apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx` |  | active | 0 | Inline editor for the free-form notes attached to a bookmark. |
| "apps/mobile/app/dashboard/bookmarks/[slug]/info::TagList" | TagList | `apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx` |  | active | 6 | Displays the tags assigned to a bookmark on the info screen. |
| "apps/mobile/app/dashboard/bookmarks/[slug]/info::ManageListsRow" | ManageListsRow | `apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx` |  | active | 0 | Row that leads to list management for the bookmark (see @apps/mobile/app/dashboard/bookmarks/[slug]/manage_lists::ListPickerPage). |
| "apps/mobile/app/dashboard/bookmarks/[slug]/info::AISummarySection" | AISummarySection | `apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx` |  | active | 0 | Section of the info screen presenting an AI-generated summary of the bookmark. |
| "apps/mobile/app/dashboard/bookmarks/[slug]/info::BookmarkActionsSection" | BookmarkActionsSection | `apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx` |  | active | 0 | Group of actions that can be performed on the bookmark from the info screen. |
| "apps/mobile/app/dashboard/bookmarks/[slug]/info::ViewBookmarkPage" | ViewBookmarkPage | `apps/mobile/app/dashboard/bookmarks/[slug]/info.tsx` |  | active | 0 | Bookmark info screen composing the title, notes, tags, lists, AI summary and actions sections. |
| "apps/mobile/app/dashboard/bookmarks/[slug]/manage_lists::ListPickerPage" | ListPickerPage | `apps/mobile/app/dashboard/bookmarks/[slug]/manage_lists.tsx` |  | placeholder | 0 | Picker screen for adding a bookmark to or removing it from lists. |
| "apps/mobile/app/dashboard/bookmarks/[slug]/manage_tags::TagPickerPage" | TagPickerPage | `apps/mobile/app/dashboard/bookmarks/[slug]/manage_tags.tsx` | action (2) | active, checked, placeholder | 0 | Picker screen for assigning or removing tags on a bookmark. |
| "apps/mobile/app/dashboard/bookmarks/new::NoteEditorPage" | NoteEditorPage | `apps/mobile/app/dashboard/bookmarks/new.tsx` |  |  | 0 | Screen for composing a new note-type bookmark. |
| "apps/mobile/app/dashboard/favourites::Favourites" | Favourites | `apps/mobile/app/dashboard/favourites.tsx` |  |  | 0 | Dashboard screen showing the user's favourited bookmarks. |
| "apps/mobile/app/dashboard/lists/[slug]/add::PickerThumbnail" | PickerThumbnail | `apps/mobile/app/dashboard/lists/[slug]/add.tsx` |  | active, checked, dark, disabled | 0 | Thumbnail item used when picking bookmarks to add to a list. |
| "apps/mobile/app/dashboard/lists/[slug]/add::AddBookmarksToListPage" | AddBookmarksToListPage | `apps/mobile/app/dashboard/lists/[slug]/add.tsx` |  | active, checked, dark, disabled | 0 | Page for selecting bookmarks and adding them to a given list. |
| "apps/mobile/app/dashboard/lists/[slug]/edit::EditListPage" | EditListPage | `apps/mobile/app/dashboard/lists/[slug]/edit.tsx` |  |  | 0 | Page for editing an existing list's details. |
| "apps/mobile/app/dashboard/lists/[slug]/index::ListView" | ListView | `apps/mobile/app/dashboard/lists/[slug]/index.tsx` |  |  | 1 | Screen displaying the contents of a single list. |
| "apps/mobile/app/dashboard/lists/[slug]/index::ListActionsMenu" | ListActionsMenu | `apps/mobile/app/dashboard/lists/[slug]/index.tsx` |  |  | 0 | Menu of actions available on a list from its view screen. |
| "apps/mobile/app/dashboard/lists/[slug]/sharing::ListSharingPage" | ListSharingPage | `apps/mobile/app/dashboard/lists/[slug]/sharing.tsx` |  |  | 0 | Page for managing sharing of a list. |
| "apps/mobile/app/dashboard/lists/new::NewListPage" | NewListPage | `apps/mobile/app/dashboard/lists/new.tsx` |  |  | 0 | Page for creating a new list. |
| "apps/mobile/app/dashboard/lists/select-parent::SelectListParentPage" | SelectListParentPage | `apps/mobile/app/dashboard/lists/select-parent.tsx` |  | placeholder | 0 | Page for choosing a parent list when nesting lists. |
| "apps/mobile/app/dashboard/settings/_layout::SettingsLayout" | SettingsLayout | `apps/mobile/app/dashboard/settings/_layout.tsx` |  |  | 0 | Layout wrapper shared by the settings screens. |
| "apps/mobile/app/dashboard/settings/bookmark-default-view::BookmarkDefaultViewSettings" | BookmarkDefaultViewSettings | `apps/mobile/app/dashboard/settings/bookmark-default-view.tsx` | mode (3) |  | 0 | Settings screen for the default view used when opening bookmarks. |
| "apps/mobile/app/dashboard/settings/index::Settings" | Settings | `apps/mobile/app/dashboard/settings/index.tsx` |  | dark | 6 | Top-level settings screen linking to the individual settings pages. |
| "apps/mobile/app/dashboard/settings/language::LanguagePage" | LanguagePage | `apps/mobile/app/dashboard/settings/language.tsx` |  |  | 0 | Settings page for choosing the app language. |
| "apps/mobile/app/dashboard/settings/offline-articles::OfflineArticles" | OfflineArticles | `apps/mobile/app/dashboard/settings/offline-articles.tsx` |  | active | 0 | Settings screen for articles stored for offline reading. |
| "apps/mobile/app/dashboard/settings/offline-lists::OfflineLists" | OfflineLists | `apps/mobile/app/dashboard/settings/offline-lists.tsx` |  |  | 0 | Settings screen for lists made available offline. |
| "apps/mobile/app/dashboard/settings/offline::DownloadProgress" | DownloadProgress | `apps/mobile/app/dashboard/settings/offline.tsx` |  |  | 0 | Progress display for offline content downloads. |
| "apps/mobile/app/dashboard/settings/offline::SectionHeader" | SectionHeader | `apps/mobile/app/dashboard/settings/offline.tsx` |  |  | 0 | Heading used to label sections within the offline settings screen. |
| "apps/mobile/app/dashboard/settings/offline::OfflineContent" | OfflineContent | `apps/mobile/app/dashboard/settings/offline.tsx` |  |  | 0 | Settings screen for managing offline content. |
| "apps/mobile/app/dashboard/settings/reader-settings::ReaderSettingsPage" | ReaderSettingsPage | `apps/mobile/app/dashboard/settings/reader-settings.tsx` |  |  | 0 | Settings page for reader-related preferences. |
| "apps/mobile/app/dashboard/settings/reading::ReaderViewSettings" | ReaderViewSettings | `apps/mobile/app/dashboard/settings/reading.tsx` |  |  | 0 | Settings screen for reader view options. |
| "apps/mobile/app/dashboard/settings/subscription::SubscriptionSettings" | SubscriptionSettings | `apps/mobile/app/dashboard/settings/subscription.tsx` |  |  | 1 | Settings screen for the user's subscription. |
| "apps/mobile/app/dashboard/settings/theme::ThemePage" | ThemePage | `apps/mobile/app/dashboard/settings/theme.tsx` |  | dark | 0 | Settings page for selecting the app theme. |
| "apps/mobile/app/dashboard/settings/toolbar-settings::ToolbarSettingsPage" | ToolbarSettingsPage | `apps/mobile/app/dashboard/settings/toolbar-settings.tsx` |  | active | 0 | Settings page for configuring the toolbar. |
| "apps/mobile/app/dashboard/settings/uploads::UploadSettings" | UploadSettings | `apps/mobile/app/dashboard/settings/uploads.tsx` |  |  | 0 | Settings screen for upload preferences. |
| "apps/mobile/app/dashboard/tags/[slug]::TagView" | TagView | `apps/mobile/app/dashboard/tags/[slug].tsx` |  |  | 0 | Screen displaying bookmarks under a single tag. |
| "apps/mobile/app/dashboard/tags/[slug]::TagActionsMenu" | TagActionsMenu | `apps/mobile/app/dashboard/tags/[slug].tsx` |  |  | 0 | Menu of actions available on a tag from its view screen. |
| "apps/mobile/app/dashboard/tags/[slug]/edit::EditTagPage" | EditTagPage | `apps/mobile/app/dashboard/tags/[slug]/edit.tsx` |  |  | 0 | Page for editing an existing tag. |
| "apps/mobile/app/dashboard/tags/new::NewTagPage" | NewTagPage | `apps/mobile/app/dashboard/tags/new.tsx` |  |  | 0 | Page for creating a new tag. |
| "apps/mobile/app/error::ErrorPage" | ErrorPage | `apps/mobile/app/error.tsx` |  |  | 0 | Route-level error screen. |
| "apps/mobile/app/index::App" | App | `apps/mobile/app/index.tsx` |  |  | 1 | Root entry screen of the mobile app. |
| "apps/mobile/app/server-address::ServerAddress" | ServerAddress | `apps/mobile/app/server-address.tsx` |  | active, disabled | 0 | Screen for entering the server address to connect to. |
| "apps/mobile/app/sharing::Sharing" | Sharing | `apps/mobile/app/sharing.tsx` |  | active | 0 | Screen handling content shared into the app. |
| "apps/mobile/app/signin::FieldRow" | FieldRow | `apps/mobile/app/signin.tsx` |  | active, placeholder | 0 | Labelled input row used in the sign-in form. |
| "apps/mobile/app/signin::Signin" | Signin | `apps/mobile/app/signin.tsx` |  | active, placeholder | 0 | Sign-in screen. |
| "apps/mobile/app/test-connection::TestConnection" | TestConnection | `apps/mobile/app/test-connection.tsx` |  |  | 0 | Screen that tests connectivity to the configured server. |
| "apps/mobile/components/ConnectionBanner::ConnectionBanner" | ConnectionBanner | `apps/mobile/components/ConnectionBanner.tsx` |  |  | 1 | Banner surfacing the current connection state. |
| "apps/mobile/components/ConnectionStatusIndicator::ConnectionStatusIndicator" | ConnectionStatusIndicator | `apps/mobile/components/ConnectionStatusIndicator.tsx` |  |  | 1 | Compact indicator of connection status. |
| "apps/mobile/components/CustomHeadersModal::CustomHeadersModal" | CustomHeadersModal | `apps/mobile/components/CustomHeadersModal.tsx` |  | dark | 0 | Modal for configuring custom request headers. |
| "apps/mobile/components/FullPageError::FullPageError" | FullPageError | `apps/mobile/components/FullPageError.tsx` |  |  | 4 | Full-screen error state component. |
| "apps/mobile/components/Logo::Logo" | Logo | `apps/mobile/components/Logo.tsx` |  |  | 3 | App logo component. |
| "apps/mobile/components/QueryPageState::QueryPageState" | QueryPageState | `apps/mobile/components/QueryPageState.tsx` |  |  | 20 | Generic page-level wrapper for a data query's state (e.g. loading, error, empty) before content renders; not bookmark-specific. |
| "apps/mobile/components/bookmarks/AttachmentBox::AttachmentBox" | AttachmentBox | `apps/mobile/components/bookmarks/AttachmentBox.tsx` |  | active, disabled | 2 | Boxed presentation of an attachment belonging to a bookmark. |
| "apps/mobile/components/bookmarks/BookmarkAssetImage::BookmarkAssetImage" | BookmarkAssetImage | `apps/mobile/components/bookmarks/BookmarkAssetImage.tsx` |  |  | 3 | Renders the image for an asset-type bookmark. |
| "apps/mobile/components/bookmarks/BookmarkAssetView::BookmarkAssetView" | BookmarkAssetView | `apps/mobile/components/bookmarks/BookmarkAssetView.tsx` |  |  | 1 | Full view for an asset-type bookmark; the asset counterpart to the link and text views. |
| "apps/mobile/components/bookmarks/BookmarkCard::BookmarkFooterMetadata" | BookmarkFooterMetadata | `apps/mobile/components/bookmarks/BookmarkCard.tsx` | align (2) | dark | 0 | Footer row of a bookmark card showing the bookmark's metadata. |
| "apps/mobile/components/bookmarks/BookmarkCard::ExpandedLinkImage" | ExpandedLinkImage | `apps/mobile/components/bookmarks/BookmarkCard.tsx` |  | dark | 0 | Expanded (larger) image treatment for a link bookmark within a card. |
| "apps/mobile/components/bookmarks/BookmarkCard::LinkPlaceholder" | LinkPlaceholder | `apps/mobile/components/bookmarks/BookmarkCard.tsx` |  | dark | 0 | Placeholder shown for a link bookmark when no image/preview is available. |
| "apps/mobile/components/bookmarks/BookmarkCard::CardActions" | CardActions | `apps/mobile/components/bookmarks/BookmarkCard.tsx` |  | dark | 0 | Action controls attached to a bookmark card. |
| "apps/mobile/components/bookmarks/BookmarkCard::CardLayout" | CardLayout | `apps/mobile/components/bookmarks/BookmarkCard.tsx` |  | dark | 0 | Card-style layout variant for presenting a bookmark. |
| "apps/mobile/components/bookmarks/BookmarkCard::ListLayout" | ListLayout | `apps/mobile/components/bookmarks/BookmarkCard.tsx` |  | dark | 0 | List-row layout variant for presenting a bookmark, alternative to the card layout. |
| "apps/mobile/components/bookmarks/BookmarkCard::SwipeAction" | SwipeAction | `apps/mobile/components/bookmarks/BookmarkCard.tsx` |  | dark | 0 | Action revealed by swiping a bookmark card. |
| "apps/mobile/components/bookmarks/BookmarkCard::CardGestures" | CardGestures | `apps/mobile/components/bookmarks/BookmarkCard.tsx` |  | dark | 0 | Gesture handling wrapper (such as swipe) around a bookmark card. |
| "apps/mobile/components/bookmarks/BookmarkCard::BookmarkCard" | BookmarkCard | `apps/mobile/components/bookmarks/BookmarkCard.tsx` |  | dark | 4 | Top-level bookmark card that composes the layouts, gestures, actions, and footer metadata in this file. |
| "apps/mobile/components/bookmarks/BookmarkContentLoading::BookmarkContentLoading" | BookmarkContentLoading | `apps/mobile/components/bookmarks/BookmarkContentLoading.tsx` |  |  | 1 | Loading state displayed while a bookmark's content is being fetched. |
| "apps/mobile/components/bookmarks/BookmarkHtmlHighlighterDom::BookmarkHtmlHighlighterDom" | BookmarkHtmlHighlighterDom | `apps/mobile/components/bookmarks/BookmarkHtmlHighlighterDom.tsx` |  | dark | 1 | DOM-based renderer of a bookmark's HTML with highlighting support. |
| "apps/mobile/components/bookmarks/BookmarkLinkPreview::BookmarkLinkBrowserPreview" | BookmarkLinkBrowserPreview | `apps/mobile/components/bookmarks/BookmarkLinkPreview.tsx` |  |  | 1 | Browser-mode preview of a link bookmark. |
| "apps/mobile/components/bookmarks/BookmarkLinkPreview::BookmarkLinkPdfPreview" | BookmarkLinkPdfPreview | `apps/mobile/components/bookmarks/BookmarkLinkPreview.tsx` |  |  | 1 | PDF-mode preview of a link bookmark. |
| "apps/mobile/components/bookmarks/BookmarkLinkPreview::BookmarkLinkReaderPreview" | BookmarkLinkReaderPreview | `apps/mobile/components/bookmarks/BookmarkLinkPreview.tsx` |  |  | 1 | Reader-mode preview of a link bookmark. |
| "apps/mobile/components/bookmarks/BookmarkLinkPreview::BookmarkLinkArchivePreview" | BookmarkLinkArchivePreview | `apps/mobile/components/bookmarks/BookmarkLinkPreview.tsx` |  |  | 1 | Archived-copy preview of a link bookmark. |
| "apps/mobile/components/bookmarks/BookmarkLinkPreview::BookmarkLinkScreenshotPreview" | BookmarkLinkScreenshotPreview | `apps/mobile/components/bookmarks/BookmarkLinkPreview.tsx` |  |  | 1 | Screenshot preview of a link bookmark. |
| "apps/mobile/components/bookmarks/BookmarkLinkTypeSelector::BookmarkLinkTypeSelector" | BookmarkLinkTypeSelector | `apps/mobile/components/bookmarks/BookmarkLinkTypeSelector.tsx` |  |  | 1 | Selector for choosing which link preview type (browser, reader, PDF, archive, screenshot) to display. |
| "apps/mobile/components/bookmarks/BookmarkLinkView::BookmarkLinkView" | BookmarkLinkView | `apps/mobile/components/bookmarks/BookmarkLinkView.tsx` |  |  | 1 | Full view for a link-type bookmark, hosting the preview variants and type selector. |
| "apps/mobile/components/bookmarks/BookmarkList::BookmarkList" | BookmarkList | `apps/mobile/components/bookmarks/BookmarkList.tsx` |  |  | 2 | Scrollable list of bookmark cards. |
| "apps/mobile/components/bookmarks/BookmarkListHeader::BookmarkListHeader" | BookmarkListHeader | `apps/mobile/components/bookmarks/BookmarkListHeader.tsx` |  |  | 4 | Header rendered above a bookmark list. |
| "apps/mobile/components/bookmarks/BookmarkTextMarkdown::BookmarkTextMarkdown" | BookmarkTextMarkdown | `apps/mobile/components/bookmarks/BookmarkTextMarkdown.tsx` | size (2) |  | 3 | Markdown renderer for a text bookmark's body. |
| "apps/mobile/components/bookmarks/BookmarkTextView::BookmarkTextView" | BookmarkTextView | `apps/mobile/components/bookmarks/BookmarkTextView.tsx` |  |  | 1 | Full view for a text-type bookmark. |
| "apps/mobile/components/bookmarks/BottomActions::ToolbarItem" | ToolbarItem | `apps/mobile/components/bookmarks/BottomActions.tsx` |  | disabled | 0 | Single item inside the bottom action toolbar. |
| "apps/mobile/components/bookmarks/BottomActions::ToolbarContainer" | ToolbarContainer | `apps/mobile/components/bookmarks/BottomActions.tsx` |  | disabled | 0 | Container that lays out the bottom toolbar items. |
| "apps/mobile/components/bookmarks/BottomActions::BottomActions" | BottomActions | `apps/mobile/components/bookmarks/BottomActions.tsx` |  | disabled | 2 | Bottom-anchored action bar for a bookmark, built from the toolbar container and items. |
| "apps/mobile/components/bookmarks/NotePreview::NotePreview" | NotePreview | `apps/mobile/components/bookmarks/NotePreview.tsx` |  |  | 3 | Preview of a note attached to a bookmark. |
| "apps/mobile/components/bookmarks/PDFViewer::PDFViewer" | PDFViewer | `apps/mobile/components/bookmarks/PDFViewer.tsx` |  | file | 2 | Embedded PDF viewer for bookmark content. |
| "apps/mobile/components/bookmarks/TagPill::TagPill" | TagPill | `apps/mobile/components/bookmarks/TagPill.tsx` |  | active, dark | 4 | Pill-shaped chip displaying a bookmark tag. |
| "apps/mobile/components/bookmarks/UpdatingBookmarkList::UpdatingBookmarkList" | UpdatingBookmarkList | `apps/mobile/components/bookmarks/UpdatingBookmarkList.tsx` |  |  | 5 | Bookmark list variant that handles live updating/refreshing of its data. |
| "apps/mobile/components/bookmarks/card/ActionBar::ActionBar" | ActionBar | `apps/mobile/components/bookmarks/card/ActionBar.tsx` |  |  | 4 | Action bar for the newer card implementation under bookmarks/card. |
| "apps/mobile/components/bookmarks/card/BookmarkCard::NoteSection" | NoteSection | `apps/mobile/components/bookmarks/card/BookmarkCard.tsx` |  |  | 0 | Section of the card that displays the bookmark's note. |
| "apps/mobile/components/bookmarks/card/BookmarkCard::FooterExtras" | FooterExtras | `apps/mobile/components/bookmarks/card/BookmarkCard.tsx` |  |  | 0 | Supplementary content placed in the card footer. |
| "apps/mobile/components/bookmarks/card/BookmarkCard::PressableSlot" | PressableSlot | `apps/mobile/components/bookmarks/card/BookmarkCard.tsx` |  |  | 0 | Pressable wrapper slot used to make a region of the card tappable. |
| "apps/mobile/components/bookmarks/card/BookmarkCard::Media" | Media | `apps/mobile/components/bookmarks/card/BookmarkCard.tsx` |  |  | 0 | Media region of the card (image or preview) in the standard size. |
| "apps/mobile/components/bookmarks/card/BookmarkCard::CompactMedia" | CompactMedia | `apps/mobile/components/bookmarks/card/BookmarkCard.tsx` |  |  | 0 | Compact-size media region for denser card presentations. |
| "apps/mobile/components/bookmarks/card/BookmarkCard::Body" | Body | `apps/mobile/components/bookmarks/card/BookmarkCard.tsx` |  |  | 0 | Main textual body of the card (title and summary area). |
| "apps/mobile/components/bookmarks/card/BookmarkCard::CompactBody" | CompactBody | `apps/mobile/components/bookmarks/card/BookmarkCard.tsx` |  |  | 0 | Compact body layout for a bookmark card, used when the card is shown in its condensed form. |
| "apps/mobile/components/bookmarks/card/BookmarkCard::Title" | Title | `apps/mobile/components/bookmarks/card/BookmarkCard.tsx` |  |  | 0 | Title text element of a bookmark card. |
| "apps/mobile/components/bookmarks/card/BookmarkCard::Root" | Root | `apps/mobile/components/bookmarks/card/BookmarkCard.tsx` |  |  | 1 | Outer container of a bookmark card that composes its sub-parts. |
| "apps/mobile/components/bookmarks/card/TagList::TagListSkeleton" | TagListSkeleton | `apps/mobile/components/bookmarks/card/TagList.tsx` |  |  | 0 | Loading placeholder shown in place of a bookmark's tag list while tags are being fetched. |
| "apps/mobile/components/bookmarks/card/TagList::TagList" | TagList | `apps/mobile/components/bookmarks/card/TagList.tsx` |  |  | 7 | Displays the tags attached to a bookmark within its card. |
| "apps/mobile/components/highlights/HighlightCard::HighlightCard" | HighlightCard | `apps/mobile/components/highlights/HighlightCard.tsx` |  | active | 5 | Card presenting a single saved highlight. |
| "apps/mobile/components/highlights/HighlightList::HighlightList" | HighlightList | `apps/mobile/components/highlights/HighlightList.tsx` |  |  | 2 | Scrollable list of highlight cards. |
| "apps/mobile/components/lists/ListFormFields::ListFormFields" | ListFormFields | `apps/mobile/components/lists/ListFormFields.tsx` |  | active | 2 | Form fields used when creating or editing a list. |
| "apps/mobile/components/lists/list-parent-field::ListParentField" | ListParentField | `apps/mobile/components/lists/list-parent-field.tsx` |  | active | 1 | Form field for choosing a parent list, supporting nested lists. |
| "apps/mobile/components/lists/list-picker::ListPicker" | ListPicker | `apps/mobile/components/lists/list-picker.tsx` | state (2) | active, disabled | 3 | Selector for picking an existing list. |
| "apps/mobile/components/lists/list-sharing-settings::RolePicker" | RolePicker | `apps/mobile/components/lists/list-sharing-settings.tsx` |  | active | 0 | Control for choosing a collaborator's role on a shared list. |
| "apps/mobile/components/lists/list-sharing-settings::Person" | Person | `apps/mobile/components/lists/list-sharing-settings.tsx` |  | active | 0 | Row representing one person who has access to a shared list. |
| "apps/mobile/components/lists/list-sharing-settings::ListSharingSettings" | ListSharingSettings | `apps/mobile/components/lists/list-sharing-settings.tsx` |  | active | 1 | Screen or panel for managing who a list is shared with and their roles. |
| "apps/mobile/components/lists/pending-list-invitations::InvitationRow" | InvitationRow | `apps/mobile/components/lists/pending-list-invitations.tsx` | role (2) |  | 1 | Row for a single pending invitation to a shared list. |
| "apps/mobile/components/lists/pending-list-invitations::PendingListInvitations" | PendingListInvitations | `apps/mobile/components/lists/pending-list-invitations.tsx` |  |  | 0 | Section listing list-sharing invitations awaiting a response. |
| "apps/mobile/components/navigation/stack::StackImpl" | StackImpl | `apps/mobile/components/navigation/stack.tsx` |  |  | 0 | Implementation of the app's stack navigator used to compose screens. |
| "apps/mobile/components/reader/ReaderPreview::ReaderPreview" | ReaderPreview | `apps/mobile/components/reader/ReaderPreview.tsx` |  |  | 1 | Preview of a bookmark's content in reader form. |
| "apps/mobile/components/search/BookmarkSearchResults::BookmarkSearchResults" | BookmarkSearchResults | `apps/mobile/components/search/BookmarkSearchResults.tsx` |  | active | 2 | Renders the bookmarks returned by a search. |
| "apps/mobile/components/search/InlineSearch::InlineSearch" | InlineSearch | `apps/mobile/components/search/InlineSearch.tsx` |  |  | 1 | Inline search input embedded within a screen. |
| "apps/mobile/components/search/SearchModeSelector::SearchModeSelector" | SearchModeSelector | `apps/mobile/components/search/SearchModeSelector.tsx` |  |  | 3 | Control for switching between available search modes. |
| "apps/mobile/components/settings/ProfileAvatarButton::ProfileAvatarButton" | ProfileAvatarButton | `apps/mobile/components/settings/ProfileAvatarButton.tsx` |  |  | 5 | Tappable avatar that opens the user's profile or settings. |
| "apps/mobile/components/settings/UsageStatsScreen::SectionLabel" | SectionLabel | `apps/mobile/components/settings/UsageStatsScreen.tsx` |  |  | 0 | Heading label for a section of the usage statistics screen. |
| "apps/mobile/components/settings/UsageStatsScreen::SectionCard" | SectionCard | `apps/mobile/components/settings/UsageStatsScreen.tsx` |  |  | 0 | Card container grouping related content on the usage statistics screen. |
| "apps/mobile/components/settings/UsageStatsScreen::MetricTile" | MetricTile | `apps/mobile/components/settings/UsageStatsScreen.tsx` |  |  | 0 | Tile displaying a single usage metric. |
| "apps/mobile/components/settings/UsageStatsScreen::ProgressRow" | ProgressRow | `apps/mobile/components/settings/UsageStatsScreen.tsx` |  |  | 0 | Row with a labeled progress indicator on the usage statistics screen. |
| "apps/mobile/components/settings/UsageStatsScreen::RankedList" | RankedList | `apps/mobile/components/settings/UsageStatsScreen.tsx` |  |  | 0 | Ordered list of ranked items within usage statistics. |
| "apps/mobile/components/settings/UsageStatsScreen::ActivityCharts" | ActivityCharts | `apps/mobile/components/settings/UsageStatsScreen.tsx` |  |  | 0 | Charts visualizing activity over time on the usage statistics screen. |
| "apps/mobile/components/settings/UsageStatsScreen::SourcesList" | SourcesList | `apps/mobile/components/settings/UsageStatsScreen.tsx` |  |  | 0 | List of content sources shown in usage statistics. |
| "apps/mobile/components/settings/UsageStatsScreen::StatsSkeleton" | StatsSkeleton | `apps/mobile/components/settings/UsageStatsScreen.tsx` |  |  | 1 | Loading placeholder for the usage statistics screen. |
| "apps/mobile/components/settings/UsageStatsScreen::UsageStatsScreen" | UsageStatsScreen | `apps/mobile/components/settings/UsageStatsScreen.tsx` |  |  | 0 | Screen composing sections, tiles, charts and lists of the user's usage statistics. |
| "apps/mobile/components/settings/UserProfileHeader::UserProfileHeader" | UserProfileHeader | `apps/mobile/components/settings/UserProfileHeader.tsx` |  |  | 1 | Header block showing the current user's profile at the top of settings. |
| "apps/mobile/components/settings/settings-list::SettingsScreen" | SettingsScreen | `apps/mobile/components/settings/settings-list.tsx` | tone (3) | active, checked | 13 | Top-level settings screen that lays out groups of settings rows. |
| "apps/mobile/components/settings/settings-list::SettingsGroup" | SettingsGroup | `apps/mobile/components/settings/settings-list.tsx` |  | active, checked | 27 | Grouped block of related settings rows. |
| "apps/mobile/components/settings/settings-list::SettingsSeparator" | SettingsSeparator | `apps/mobile/components/settings/settings-list.tsx` |  | active, checked | 27 | Divider between rows or groups in the settings list. |
| "apps/mobile/components/settings/settings-list::SettingsNavigationRow" | SettingsNavigationRow | `apps/mobile/components/settings/settings-list.tsx` |  | active, checked | 13 | Settings row that navigates to another screen. |
| "apps/mobile/components/settings/settings-list::SettingsToggleRow" | SettingsToggleRow | `apps/mobile/components/settings/settings-list.tsx` |  | active, checked | 3 | Settings row with an on/off toggle. |
| "apps/mobile/components/settings/settings-list::SettingsMenuRow" | SettingsMenuRow | `apps/mobile/components/settings/settings-list.tsx` |  |  | 0 | Settings row that opens a menu of options. |
| "apps/mobile/components/settings/settings-list::SettingsChoiceRow" | SettingsChoiceRow | `apps/mobile/components/settings/settings-list.tsx` |  | active, checked | 5 | Settings row for selecting one choice among several. |
| "apps/mobile/components/settings/settings-list::SettingsValueRow" | SettingsValueRow | `apps/mobile/components/settings/settings-list.tsx` |  | active, checked | 7 | Settings row displaying a read-only value. |
| "apps/mobile/components/settings/settings-list::SettingsActionRow" | SettingsActionRow | `apps/mobile/components/settings/settings-list.tsx` |  | active, checked | 14 | Settings row that triggers an action when tapped. |
| "apps/mobile/components/sharing/ErrorAnimation::ErrorAnimation" | ErrorAnimation | `apps/mobile/components/sharing/ErrorAnimation.tsx` |  |  | 1 | Animated error indicator shown in the mobile sharing flow when an operation fails. |
| "apps/mobile/components/sharing/LoadingAnimation::LoadingAnimation" | LoadingAnimation | `apps/mobile/components/sharing/LoadingAnimation.tsx` |  |  | 1 | Animated loading indicator for in-progress states in the mobile sharing flow. |
| "apps/mobile/components/sharing/SuccessAnimation::Particle" | Particle | `apps/mobile/components/sharing/SuccessAnimation.tsx` |  |  | 0 | Single animated particle used as a building block of the success animation. |
| "apps/mobile/components/sharing/SuccessAnimation::SuccessAnimation" | SuccessAnimation | `apps/mobile/components/sharing/SuccessAnimation.tsx` |  |  | 1 | Animated success confirmation shown when a sharing action completes. |
| "apps/mobile/components/ui/ActionButton::ActionButton" | ActionButton | `apps/mobile/components/ui/ActionButton.tsx` |  |  | 88 | Button variant intended for a prominent action within mobile screens. |
| "apps/mobile/components/ui/AndroidSearchBar::AndroidSearchBar" | AndroidSearchBar | `apps/mobile/components/ui/AndroidSearchBar.tsx` |  |  | 1 | Android-specific search bar for filtering content on mobile. |
| "apps/mobile/components/ui/AppIcon::AppIcon" | AppIcon | `apps/mobile/components/ui/AppIcon.tsx` |  |  | 39 | Renders an application icon tile in the mobile UI. |
| "apps/mobile/components/ui/AppIcon::SelectionIndicator" | SelectionIndicator | `apps/mobile/components/ui/AppIcon.tsx` |  |  | 3 | Overlay marking an AppIcon as selected. |
| "apps/mobile/components/ui/Avatar::Avatar" | Avatar | `apps/mobile/components/ui/Avatar.tsx` |  |  | 3 | Displays a user or entity avatar image or fallback. |
| "apps/mobile/components/ui/Button::Button" | Button | `apps/mobile/components/ui/Button.tsx` | variant (5), size (5) | active, dark | 205 | Base pressable button primitive for the mobile app. |
| "apps/mobile/components/ui/ChevronRight::ChevronRight" | ChevronRight | `apps/mobile/components/ui/ChevronRight.tsx` |  |  | 17 | Right-pointing chevron icon used to signal navigation affordances. |
| "apps/mobile/components/ui/Divider::Divider" | Divider | `apps/mobile/components/ui/Divider.tsx` | orientation (2) | dark | 0 | Thin horizontal rule separating content sections. |
| "apps/mobile/components/ui/EmptyState::EmptyState" | EmptyState | `apps/mobile/components/ui/EmptyState.tsx` |  |  | 8 | Placeholder shown when a list or screen has no content. |
| "apps/mobile/components/ui/FAB/FAB.ios::FAB" | FAB | `apps/mobile/components/ui/FAB/FAB.ios.tsx` |  |  | 0 | iOS-specific floating action button. |
| "apps/mobile/components/ui/FAB/FAB::FAB" | FAB | `apps/mobile/components/ui/FAB/FAB.tsx` |  |  | 0 | Default floating action button for triggering a primary action. |
| "apps/mobile/components/ui/FullPageSpinner::FullPageSpinner" | FullPageSpinner | `apps/mobile/components/ui/FullPageSpinner.tsx` |  | dark | 21 | Full-screen loading spinner while a screen's data is being fetched. |
| "apps/mobile/components/ui/GroupedList::GroupedSection" | GroupedSection | `apps/mobile/components/ui/GroupedList.tsx` |  | active | 22 | Container grouping related rows in a settings-style list. |
| "apps/mobile/components/ui/GroupedList::GroupedHeader" | GroupedHeader | `apps/mobile/components/ui/GroupedList.tsx` |  | active | 1 | Section header label for a grouped list. |
| "apps/mobile/components/ui/GroupedList::GroupedListRow" | GroupedListRow | `apps/mobile/components/ui/GroupedList.tsx` |  | active | 4 | Single row inside a grouped list section. |
| "apps/mobile/components/ui/GroupedList::RowSeparator" | RowSeparator | `apps/mobile/components/ui/GroupedList.tsx` |  | active | 20 | Separator line drawn between grouped list rows. |
| "apps/mobile/components/ui/GroupedList::NavigationRow" | NavigationRow | `apps/mobile/components/ui/GroupedList.tsx` |  | active | 3 | Grouped list row that navigates to another screen when pressed. |
| "apps/mobile/components/ui/Input::Input" | Input | `apps/mobile/components/ui/Input.tsx` |  | placeholder | 80 | Text input field primitive for forms on mobile. |
| "apps/mobile/components/ui/SearchInput/SearchInput.ios::SearchInput" | SearchInput | `apps/mobile/components/ui/SearchInput/SearchInput.ios.tsx` |  | active, dark, placeholder | 4 | iOS-specific search text input. |
| "apps/mobile/components/ui/SearchInput/SearchInput::SearchInput" | SearchInput | `apps/mobile/components/ui/SearchInput/SearchInput.tsx` |  | placeholder | 4 | Default search text input for filtering lists. |
| "apps/mobile/components/ui/SegmentedControl::SegmentedControl" | SegmentedControl | `apps/mobile/components/ui/SegmentedControl.tsx` |  | active, dark | 1 | Control for switching between a small set of mutually exclusive options. |
| "apps/mobile/components/ui/SheetHeader::HeaderTextButton" | HeaderTextButton | `apps/mobile/components/ui/SheetHeader.tsx` |  | active | 10 | Text-only button placed in a sheet header, such as cancel or done. |
| "apps/mobile/components/ui/SheetHeader::SheetHeader" | SheetHeader | `apps/mobile/components/ui/SheetHeader.tsx` |  | active | 6 | Header bar for modal sheets, holding a title and header actions. |
| "apps/mobile/components/ui/Skeleton::Skeleton" | Skeleton | `apps/mobile/components/ui/Skeleton.tsx` |  |  | 70 | Loading placeholder block that stands in for content while it loads. |
| "apps/mobile/components/ui/Text::Text" | Text | `apps/mobile/components/ui/Text.tsx` | variant (11), color (4) |  | 239 | Themed text primitive used for typography across the mobile app. |
| "apps/mobile/components/ui/Toast::ActionToast" | ActionToast | `apps/mobile/components/ui/Toast.tsx` | toast (4), position (2) | dark | 0 | Transient toast notification that includes an actionable button. |
| "apps/mobile/components/ui/emoji-picker::EmojiCell" | EmojiCell | `apps/mobile/components/ui/emoji-picker.tsx` |  | active, disabled | 0 | Single selectable emoji cell within the emoji picker grid. |
| "apps/mobile/components/ui/emoji-picker::EmojiPicker" | EmojiPicker | `apps/mobile/components/ui/emoji-picker.tsx` |  | active, disabled | 2 | Grid picker for choosing an emoji. |
| "apps/mobile/lib/client-config::ClientConfigProvider" | ClientConfigProvider | `apps/mobile/lib/client-config.tsx` |  |  | 2 | Context provider supplying client configuration to the mobile app. |
| "apps/mobile/lib/i18n/provider::I18nProvider" | I18nProvider | `apps/mobile/lib/i18n/provider.tsx` |  |  | 3 | Context provider for internationalisation and translations. |
| "apps/mobile/lib/providers::Providers" | Providers | `apps/mobile/lib/providers.tsx` |  |  | 4 | Composes the app-level providers wrapping the mobile app. |
| "apps/mobile/lib/readerSettings::ReaderSettingsProvider" | ReaderSettingsProvider | `apps/mobile/lib/readerSettings.tsx` |  |  | 4 | Context provider for user reader settings. |
| "apps/mobile/lib/useConnectionStatus::ConnectionStatusProvider" | ConnectionStatusProvider | `apps/mobile/lib/useConnectionStatus.tsx` |  |  | 1 | Context provider exposing network connection status. |
| "apps/web/app/admin/admin_tools/page::AdminToolsPage" | AdminToolsPage | `apps/web/app/admin/admin_tools/page.tsx` |  |  | 0 | Web admin page offering administrative tools. |
| "apps/web/app/admin/background_jobs/page::BackgroundJobsPage" | BackgroundJobsPage | `apps/web/app/admin/background_jobs/page.tsx` |  |  | 0 | Web admin page for viewing background jobs. |
| "apps/web/app/admin/layout::AdminLayout" | AdminLayout | `apps/web/app/admin/layout.tsx` |  |  | 0 | Shared layout wrapping the web admin pages. |
| "apps/web/app/admin/overview/page::AdminOverviewPage" | AdminOverviewPage | `apps/web/app/admin/overview/page.tsx` |  |  | 0 | Admin overview page; the summary view within the admin area. |
| "apps/web/app/admin/page::AdminHomepage" | AdminHomepage | `apps/web/app/admin/page.tsx` |  |  | 0 | Entry page for the admin section. |
| "apps/web/app/admin/users/page::AdminUsersPage" | AdminUsersPage | `apps/web/app/admin/users/page.tsx` |  |  | 0 | Admin page for managing users. |
| "apps/web/app/check-email/page::CheckEmailPage" | CheckEmailPage | `apps/web/app/check-email/page.tsx` |  |  | 0 | Auth flow page shown after an action that requires the user to check their email. |
| "apps/web/app/dashboard/@modal/(.)preview/[bookmarkId]/page::BookmarkPreviewPage" | BookmarkPreviewPage | `apps/web/app/dashboard/@modal/(.)preview/[bookmarkId]/page.tsx` |  |  | 0 | Intercepted-route version of the bookmark preview, rendered as a modal over the dashboard for a given bookmarkId. |
| "apps/web/app/dashboard/@modal/(.)preview/layout::BookmarkPreviewDialogLayout" | BookmarkPreviewDialogLayout | `apps/web/app/dashboard/@modal/(.)preview/layout.tsx` |  |  | 0 | Dialog layout wrapping the modal bookmark preview route in the dashboard's parallel modal slot. |
| "apps/web/app/dashboard/archive/page::ArchivedBookmarkPage" | ArchivedBookmarkPage | `apps/web/app/dashboard/archive/page.tsx` |  |  | 0 | Dashboard page listing archived bookmarks. |
| "apps/web/app/dashboard/bookmarks/page::BookmarksPage" | BookmarksPage | `apps/web/app/dashboard/bookmarks/page.tsx` |  |  | 0 | Main dashboard page listing the user's bookmarks. |
| "apps/web/app/dashboard/error::Error" | Error | `apps/web/app/dashboard/error.tsx` |  |  | 0 | Error boundary page for the dashboard route segment. |
| "apps/web/app/dashboard/favourites/page::FavouritesBookmarkPage" | FavouritesBookmarkPage | `apps/web/app/dashboard/favourites/page.tsx` |  |  | 0 | Dashboard page listing bookmarks marked as favourites. |
| "apps/web/app/dashboard/feeds/[feedId]/page::FeedPage" | FeedPage | `apps/web/app/dashboard/feeds/[feedId]/page.tsx` |  |  | 0 | Dashboard page showing the contents of a single feed identified by feedId. |
| "apps/web/app/dashboard/highlights/page::HighlightsPage" | HighlightsPage | `apps/web/app/dashboard/highlights/page.tsx` |  |  | 3 | Dashboard page listing the user's highlights. |
| "apps/web/app/dashboard/layout::Dashboard" | Dashboard | `apps/web/app/dashboard/layout.tsx` |  |  | 0 | Layout shell for all dashboard routes. |
| "apps/web/app/dashboard/lists/[listId]/page::ListPage" | ListPage | `apps/web/app/dashboard/lists/[listId]/page.tsx` |  |  | 0 | Dashboard page showing a single list identified by listId. |
| "apps/web/app/dashboard/lists/page::ListsPage" | ListsPage | `apps/web/app/dashboard/lists/page.tsx` |  |  | 0 | Dashboard page listing all of the user's lists. |
| "apps/web/app/dashboard/not-found::NotFound" | NotFound | `apps/web/app/dashboard/not-found.tsx` |  | dark | 1 | Not-found page scoped to the dashboard route segment. |
| "apps/web/app/dashboard/preview/[bookmarkId]/page::BookmarkPreviewPage" | BookmarkPreviewPage | `apps/web/app/dashboard/preview/[bookmarkId]/page.tsx` |  |  | 0 | Full-page bookmark preview for a given bookmarkId, used when the route is loaded directly rather than as a modal. |
| "apps/web/app/dashboard/search/page::SearchComp" | SearchComp | `apps/web/app/dashboard/search/page.tsx` |  |  | 0 | Search component rendered within the dashboard search page. |
| "apps/web/app/dashboard/search/page::SearchPage" | SearchPage | `apps/web/app/dashboard/search/page.tsx` |  |  | 0 | Dashboard search page that hosts the search component. |
| "apps/web/app/dashboard/tags/[tagId]/page::TagPage" | TagPage | `apps/web/app/dashboard/tags/[tagId]/page.tsx` |  |  | 0 | Dashboard page showing bookmarks for a single tag identified by tagId. |
| "apps/web/app/dashboard/tags/page::TagsPage" | TagsPage | `apps/web/app/dashboard/tags/page.tsx` |  |  | 0 | Dashboard page listing all tags. |
| "apps/web/app/forgot-password/page::ForgotPasswordPage" | ForgotPasswordPage | `apps/web/app/forgot-password/page.tsx` |  |  | 0 | Auth page for starting a password-reset request. |
| "apps/web/app/invite/[token]/page::InvitePage" | InvitePage | `apps/web/app/invite/[token]/page.tsx` |  |  | 0 | Page for accepting an invitation via a token in the URL. |
| "apps/web/app/layout::RootLayout" | RootLayout | `apps/web/app/layout.tsx` |  |  | 0 | Root layout for the entire web app. |
| "apps/web/app/logout/page::Logout" | Logout | `apps/web/app/logout/page.tsx` |  |  | 0 | Page that handles signing the user out. |
| "apps/web/app/not-found::RootNotFound" | RootNotFound | `apps/web/app/not-found.tsx` |  |  | 0 | App-wide not-found page. |
| "apps/web/app/public/layout::PublicLayout" | PublicLayout | `apps/web/app/public/layout.tsx` |  |  | 0 | Layout for publicly accessible routes that do not require sign-in. |
| "apps/web/app/public/lists/[listId]/not-found::PublicListPageNotFound" | PublicListPageNotFound | `apps/web/app/public/lists/[listId]/not-found.tsx` |  | focus-visible | 0 | Not-found page for a public list that does not exist or is unavailable. |
| "apps/web/app/public/lists/[listId]/page::PublicListPage" | PublicListPage | `apps/web/app/public/lists/[listId]/page.tsx` |  |  | 0 | Publicly shared view of a list identified by listId. |
| "apps/web/app/reader/[bookmarkId]/page::ReaderViewPage" | ReaderViewPage | `apps/web/app/reader/[bookmarkId]/page.tsx` |  | hover, supports-[backdrop-filter] | 0 | Reader view page for reading a single bookmark's content by bookmarkId. |
| "apps/web/app/reader/layout::ReaderLayout" | ReaderLayout | `apps/web/app/reader/layout.tsx` |  |  | 0 | Layout shell for the reader routes. |
| "apps/web/app/reset-password/page::ResetPasswordPage" | ResetPasswordPage | `apps/web/app/reset-password/page.tsx` |  |  | 0 | Auth page for setting a new password. |
| "apps/web/app/settings/ai/page::AISettingsPage" | AISettingsPage | `apps/web/app/settings/ai/page.tsx` |  |  | 0 | Settings page for AI-related options. |
| "apps/web/app/settings/api-keys/page::ApiKeysPage" | ApiKeysPage | `apps/web/app/settings/api-keys/page.tsx` |  |  | 0 | Settings page for managing API keys. |
| "apps/web/app/settings/assets/layout::AssetsLayout" | AssetsLayout | `apps/web/app/settings/assets/layout.tsx` |  |  | 0 | Layout for the assets section of settings. |
| "apps/web/app/settings/assets/page::AssetThumbnail" | AssetThumbnail | `apps/web/app/settings/assets/page.tsx` |  | hover | 0 | Thumbnail element for an individual asset on the assets settings page. |
| "apps/web/app/settings/assets/page::AssetRow" | AssetRow | `apps/web/app/settings/assets/page.tsx` |  | hover | 0 | Row element representing a single asset on the assets settings page. |
| "apps/web/app/settings/assets/page::AssetsSettingsPage" | AssetsSettingsPage | `apps/web/app/settings/assets/page.tsx` |  | hover | 0 | Settings page listing stored assets, composed of asset rows and thumbnails. |
| "apps/web/app/settings/backups/page::BackupsPage" | BackupsPage | `apps/web/app/settings/backups/page.tsx` |  |  | 0 | Settings page for backups. |
| "apps/web/app/settings/broken-links/layout::BrokenLinksLayout" | BrokenLinksLayout | `apps/web/app/settings/broken-links/layout.tsx` |  |  | 0 | Layout for the broken-links section of settings. |
| "apps/web/app/settings/broken-links/page::IssueBadge" | IssueBadge | `apps/web/app/settings/broken-links/page.tsx` | issue (5), action (2) | dark, disabled, hover | 0 | Small status badge used within @apps/web/app/settings/broken-links/page::BrokenLinksPage to label the kind of issue detected for a link. |
| "apps/web/app/settings/broken-links/page::BrokenLinksPage" | BrokenLinksPage | `apps/web/app/settings/broken-links/page.tsx` |  | dark, disabled, hover | 0 | Settings page that lists bookmarks whose links are broken or problematic so the user can review them. |
| "apps/web/app/settings/cleanups/page::CleanupsPage" | CleanupsPage | `apps/web/app/settings/cleanups/page.tsx` |  |  | 0 | Settings page for running cleanup actions on the user's bookmark collection. |
| "apps/web/app/settings/feeds/page::FeedSettingsPage" | FeedSettingsPage | `apps/web/app/settings/feeds/page.tsx` |  |  | 0 | Settings page for managing feed subscriptions. |
| "apps/web/app/settings/import/[sessionId]/page::ImportSessionDetailPage" | ImportSessionDetailPage | `apps/web/app/settings/import/[sessionId]/page.tsx` |  |  | 0 | Detail view for a single import session, reached from @apps/web/app/settings/import/page::ImportSettingsPage. |
| "apps/web/app/settings/import/page::ImportSettingsPage" | ImportSettingsPage | `apps/web/app/settings/import/page.tsx` |  |  | 0 | Settings page for importing bookmarks and viewing past import sessions. |
| "apps/web/app/settings/info/page::InfoPage" | InfoPage | `apps/web/app/settings/info/page.tsx` |  |  | 0 | Settings page showing informational details about the account or installation. |
| "apps/web/app/settings/layout::SettingsLayout" | SettingsLayout | `apps/web/app/settings/layout.tsx` |  |  | 0 | Shared layout wrapping every settings route, providing the settings navigation and page frame. |
| "apps/web/app/settings/page::SettingsHomepage" | SettingsHomepage | `apps/web/app/settings/page.tsx` |  |  | 0 | Landing page of the settings section. |
| "apps/web/app/settings/preferences/page::PreferencesPage" | PreferencesPage | `apps/web/app/settings/preferences/page.tsx` |  |  | 0 | Settings page for user preferences. |
| "apps/web/app/settings/reading/page::ReadingPage" | ReadingPage | `apps/web/app/settings/reading/page.tsx` |  |  | 0 | Settings page for reading-related options. |
| "apps/web/app/settings/rules/layout::RulesLayout" | RulesLayout | `apps/web/app/settings/rules/layout.tsx` |  |  | 0 | Layout wrapper for the rules settings section. |
| "apps/web/app/settings/rules/page::RulesSettingsPage" | RulesSettingsPage | `apps/web/app/settings/rules/page.tsx` |  |  | 0 | Settings page for defining and managing automation rules. |
| "apps/web/app/settings/stats/layout::StatsLayout" | StatsLayout | `apps/web/app/settings/stats/layout.tsx` |  |  | 0 | Layout wrapper for the stats settings section. |
| "apps/web/app/settings/stats/page::ColumnChart" | ColumnChart | `apps/web/app/settings/stats/page.tsx` |  | dark, data-[state=checked], focus-visible, group-hover, hover | 0 | Column chart visualization used on @apps/web/app/settings/stats/page::StatsPage. |
| "apps/web/app/settings/stats/page::BarRow" | BarRow | `apps/web/app/settings/stats/page.tsx` |  | dark, data-[state=checked], focus-visible, group-hover, hover | 0 | Single horizontal bar row used to display one labeled value within the stats visualizations. |
| "apps/web/app/settings/stats/page::BookmarksAddedStat" | BookmarksAddedStat | `apps/web/app/settings/stats/page.tsx` |  | dark, data-[state=checked], focus-visible, group-hover, hover | 0 | Stat block reporting the number of bookmarks added, shown on @apps/web/app/settings/stats/page::StatsPage. |
| "apps/web/app/settings/stats/page::StatsPage" | StatsPage | `apps/web/app/settings/stats/page.tsx` |  | dark, data-[state=checked], focus-visible, group-hover, hover | 0 | Settings page presenting usage statistics about the user's bookmarks. |
| "apps/web/app/settings/subscription/page::SubscriptionPage" | SubscriptionPage | `apps/web/app/settings/subscription/page.tsx` |  |  | 0 | Settings page for viewing and managing the user's subscription. |
| "apps/web/app/settings/webhooks/page::WebhookSettingsPage" | WebhookSettingsPage | `apps/web/app/settings/webhooks/page.tsx` |  |  | 0 | Settings page for configuring webhooks. |
| "apps/web/app/signin/page::SignInPage" | SignInPage | `apps/web/app/signin/page.tsx` |  |  | 1 | Authentication page where existing users sign in. |
| "apps/web/app/signup/page::SignUpPage" | SignUpPage | `apps/web/app/signup/page.tsx` |  |  | 0 | Authentication page where new users create an account. |
| "apps/web/app/verify-email/page::VerifyEmailPage" | VerifyEmailPage | `apps/web/app/verify-email/page.tsx` |  |  | 0 | Page handling email verification after sign-up. |
| "apps/web/components/DemoModeBanner::DemoModeBanner" | DemoModeBanner | `apps/web/components/DemoModeBanner.tsx` |  |  | 1 | Banner shown when the app is running in demo mode. |
| "apps/web/components/KarakeepIcon::KarakeepLogo" | KarakeepLogo | `apps/web/components/KarakeepIcon.tsx` |  |  | 8 | Karakeep brand logo mark used across the web app. |
| "apps/web/components/admin/AddUserDialog::AddUserDialog" | AddUserDialog | `apps/web/components/admin/AddUserDialog.tsx` |  |  | 1 | Admin dialog for creating a new user account. |
| "apps/web/components/admin/AdminCard::AdminCard" | AdminCard | `apps/web/components/admin/AdminCard.tsx` |  |  | 14 | Card container used to group content on admin screens. |
| "apps/web/components/admin/AdminNotices::AdminNotices" | AdminNotices | `apps/web/components/admin/AdminNotices.tsx` | level (3) |  | 1 | Admin component surfacing notices that require operator attention. |
| "apps/web/components/admin/AdminNotices::AdminNoticeBadge" | AdminNoticeBadge | `apps/web/components/admin/AdminNotices.tsx` |  |  | 1 | Badge indicating pending admin notices, paired with @apps/web/components/admin/AdminNotices::AdminNotices. |
| "apps/web/components/admin/AdminsOnly::AdminsOnly" | AdminsOnly | `apps/web/components/admin/AdminsOnly.tsx` |  |  | 1 | Guard wrapper that renders its children only for admin users. |
| "apps/web/components/admin/BackgroundJobs::JobStatusExplanation" | JobStatusExplanation | `apps/web/components/admin/BackgroundJobs.tsx` |  | dark | 0 | Explanatory text describing what each background job status means. |
| "apps/web/components/admin/BackgroundJobs::JobCardSkeleton" | JobCardSkeleton | `apps/web/components/admin/BackgroundJobs.tsx` |  | dark | 0 | Loading placeholder shown in place of @apps/web/components/admin/BackgroundJobs::JobCard while job data loads. |
| "apps/web/components/admin/BackgroundJobs::JobCard" | JobCard | `apps/web/components/admin/BackgroundJobs.tsx` |  | dark | 0 | Card displaying the status of a single background job queue. |
| "apps/web/components/admin/BackgroundJobs::BackgroundJobs" | BackgroundJobs | `apps/web/components/admin/BackgroundJobs.tsx` |  | dark | 1 | Admin section listing background job queues and their status. |
| "apps/web/components/admin/BasicStats::ReleaseInfo" | ReleaseInfo | `apps/web/components/admin/BasicStats.tsx` |  | dark | 0 | Displays release and version information for the running instance. |
| "apps/web/components/admin/BasicStats::StatsSkeleton" | StatsSkeleton | `apps/web/components/admin/BasicStats.tsx` |  | dark | 1 | Loading placeholder for @apps/web/components/admin/BasicStats::BasicStats. |
| "apps/web/components/admin/BasicStats::BasicStats" | BasicStats | `apps/web/components/admin/BasicStats.tsx` |  | dark | 1 | Admin section showing basic instance-wide statistics. |
| "apps/web/components/admin/BookmarkDebugger::BookmarkDebugger" | BookmarkDebugger | `apps/web/components/admin/BookmarkDebugger.tsx` | status (3) | hover | 1 | Admin tool for inspecting and debugging an individual bookmark. |
| "apps/web/components/admin/CreateInviteDialog::CreateInviteDialog" | CreateInviteDialog | `apps/web/components/admin/CreateInviteDialog.tsx` |  |  | 1 | Admin dialog for creating a user invitation. |
| "apps/web/components/admin/InvitesList::InvitesList" | InvitesList | `apps/web/components/admin/InvitesList.tsx` |  | dark | 1 | Admin list of outstanding invitations, created via @apps/web/components/admin/CreateInviteDialog::CreateInviteDialog. |
| "apps/web/components/admin/InvitesListSkeleton::InvitesListSkeleton" | InvitesListSkeleton | `apps/web/components/admin/InvitesListSkeleton.tsx` |  |  | 1 | Loading placeholder shown in the admin area while the invites list is being fetched. |
| "apps/web/components/admin/ResetPasswordDialog::ResetPasswordDialog" | ResetPasswordDialog | `apps/web/components/admin/ResetPasswordDialog.tsx` |  | open | 1 | Admin dialog for resetting a user's password. |
| "apps/web/components/admin/ServiceConnections::ConnectionStatus" | ConnectionStatus | `apps/web/components/admin/ServiceConnections.tsx` |  | dark | 2 | Indicator showing the current status of a single service connection within @apps/web/components/admin/ServiceConnections::ServiceConnections. |
| "apps/web/components/admin/ServiceConnections::ConnectionsSkeleton" | ConnectionsSkeleton | `apps/web/components/admin/ServiceConnections.tsx` |  | dark | 0 | Loading placeholder for the service connections panel. |
| "apps/web/components/admin/ServiceConnections::ServiceConnections" | ServiceConnections | `apps/web/components/admin/ServiceConnections.tsx` |  | dark | 1 | Admin panel listing connected external services and their statuses. |
| "apps/web/components/admin/UpdateUserDialog::UpdateUserDialog" | UpdateUserDialog | `apps/web/components/admin/UpdateUserDialog.tsx` | currentRole (2) | open | 1 | Admin dialog for editing an existing user's details. |
| "apps/web/components/admin/UserList::UserRow" | UserRow | `apps/web/components/admin/UserList.tsx` |  | dark | 0 | Single user entry rendered inside @apps/web/components/admin/UserList::UsersSection. |
| "apps/web/components/admin/UserList::UsersSection" | UsersSection | `apps/web/components/admin/UserList.tsx` |  | dark | 0 | Admin section listing all users, composed of @apps/web/components/admin/UserList::UserRow items. |
| "apps/web/components/admin/UserListSkeleton::UserListSkeleton" | UserListSkeleton | `apps/web/components/admin/UserListSkeleton.tsx` |  |  | 1 | Loading placeholder shown while the admin user list is being fetched. |
| "apps/web/components/dashboard/BulkBookmarksAction::BulkBookmarksAction" | BulkBookmarksAction | `apps/web/components/dashboard/BulkBookmarksAction.tsx` |  | dark, motion-reduce | 1 | Action controls applied to multiple selected bookmarks at once in the dashboard. |
| "apps/web/components/dashboard/EditableText::EditMode" | EditMode | `apps/web/components/dashboard/EditableText.tsx` |  |  | 0 | Editing state of @apps/web/components/dashboard/EditableText::EditableText, exposing an input for changing the text. |
| "apps/web/components/dashboard/EditableText::ViewMode" | ViewMode | `apps/web/components/dashboard/EditableText.tsx` |  |  | 0 | Read-only display state of @apps/web/components/dashboard/EditableText::EditableText. |
| "apps/web/components/dashboard/EditableText::EditableText" | EditableText | `apps/web/components/dashboard/EditableText.tsx` |  |  | 1 | Inline text that toggles between @apps/web/components/dashboard/EditableText::ViewMode and @apps/web/components/dashboard/EditableText::EditMode. |
| "apps/web/components/dashboard/ErrorFallback::ErrorFallback" | ErrorFallback | `apps/web/components/dashboard/ErrorFallback.tsx` |  | dark | 2 | Fallback UI rendered in the dashboard when a rendering error occurs. |
| "apps/web/components/dashboard/GlobalActions::GlobalActions" | GlobalActions | `apps/web/components/dashboard/GlobalActions.tsx` |  |  | 1 | Dashboard-wide action controls available independent of the current view. |
| "apps/web/components/dashboard/KeyboardShortcutsDialog::ShortcutRow" | ShortcutRow | `apps/web/components/dashboard/KeyboardShortcutsDialog.tsx` |  | open | 0 | Single shortcut entry inside @apps/web/components/dashboard/KeyboardShortcutsDialog::ShortcutSection. |
| "apps/web/components/dashboard/KeyboardShortcutsDialog::ShortcutSection" | ShortcutSection | `apps/web/components/dashboard/KeyboardShortcutsDialog.tsx` |  | open | 0 | Grouped list of related shortcuts within @apps/web/components/dashboard/KeyboardShortcutsDialog::KeyboardShortcutsDialog. |
| "apps/web/components/dashboard/KeyboardShortcutsDialog::KeyboardShortcutsDialog" | KeyboardShortcutsDialog | `apps/web/components/dashboard/KeyboardShortcutsDialog.tsx` |  | open | 2 | Dialog presenting the dashboard's available keyboard shortcuts. |
| "apps/web/components/dashboard/ReportProblemDialog::ReportProblemDialog" | ReportProblemDialog | `apps/web/components/dashboard/ReportProblemDialog.tsx` |  | hover | 1 | Dialog allowing users to report a problem from the dashboard. |
| "apps/web/components/dashboard/SortOrderToggle::SortOrderToggle" | SortOrderToggle | `apps/web/components/dashboard/SortOrderToggle.tsx` |  |  | 1 | Control for switching the sort order of the displayed bookmarks. |
| "apps/web/components/dashboard/UploadDropzone::UploadDropzone" | UploadDropzone | `apps/web/components/dashboard/UploadDropzone.tsx` |  |  | 1 | Drag-and-drop target for uploading files into the dashboard. |
| "apps/web/components/dashboard/ViewOptions::ViewOptions" | ViewOptions | `apps/web/components/dashboard/ViewOptions.tsx` | fit (2) |  | 1 | Controls for adjusting how bookmarks are displayed in the dashboard. |
| "apps/web/components/dashboard/bookmarks/AssetCard::AssetImage" | AssetImage | `apps/web/components/dashboard/bookmarks/AssetCard.tsx` |  |  | 0 | Image rendering used within @apps/web/components/dashboard/bookmarks/AssetCard::AssetCard. |
| "apps/web/components/dashboard/bookmarks/AssetCard::AssetCard" | AssetCard | `apps/web/components/dashboard/bookmarks/AssetCard.tsx` |  |  | 1 | Card representing an asset-type bookmark. |
| "apps/web/components/dashboard/bookmarks/BookmarkActionBar::FavouriteButton" | FavouriteButton | `apps/web/components/dashboard/bookmarks/BookmarkActionBar.tsx` |  |  | 2 | Toggle for marking a bookmark as a favourite, part of @apps/web/components/dashboard/bookmarks/BookmarkActionBar::BookmarkActionBar. |
| "apps/web/components/dashboard/bookmarks/BookmarkActionBar::BookmarkActionBar" | BookmarkActionBar | `apps/web/components/dashboard/bookmarks/BookmarkActionBar.tsx` |  |  | 2 | Bar of per-bookmark actions, including @apps/web/components/dashboard/bookmarks/BookmarkActionBar::FavouriteButton. |
| "apps/web/components/dashboard/bookmarks/BookmarkCard::BookmarkCard" | BookmarkCard | `apps/web/components/dashboard/bookmarks/BookmarkCard.tsx` |  |  | 4 | Card representing a single bookmark in the dashboard. |
| "apps/web/components/dashboard/bookmarks/BookmarkFavicon::BookmarkFavicon" | BookmarkFavicon | `apps/web/components/dashboard/bookmarks/BookmarkFavicon.tsx` |  |  | 2 | Displays the favicon associated with a bookmark. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::KeyboardPreviewLink" | KeyboardPreviewLink | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | Keyboard-accessible link for opening a bookmark preview from a layout-adapting card. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::NoteTypeRow" | NoteTypeRow | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | Row variant used for note-type bookmarks within the layout-adapting card. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::BottomRow" | BottomRow | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | Bottom section of the layout-adapting card holding supplementary bookmark information. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::OwnerIndicator" | OwnerIndicator | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | Marker showing the owner of a bookmark on the layout-adapting card. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::BulkEditSelectionOverlay" | BulkEditSelectionOverlay | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | Overlay shown on a card when bulk-edit selection mode is active. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::DragHandle" | DragHandle | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | Handle used to drag and reorder a bookmark card. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::CardHoverActions" | CardHoverActions | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | Actions revealed when hovering over a bookmark card. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::CompactRowActions" | CompactRowActions | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | Actions available on a bookmark row in @apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::CompactView. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::CardToolbar" | CardToolbar | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | Toolbar grouping the controls attached to a bookmark card. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::ListView" | ListView | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | List layout variant of the bookmark card. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::GridView" | GridView | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | Grid layout variant of the bookmark card. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::CompactView" | CompactView | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 0 | Compact layout variant of the bookmark card, using @apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::CompactRowActions. |
| "apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard::BookmarkLayoutAdaptingCard" | BookmarkLayoutAdaptingCard | `apps/web/components/dashboard/bookmarks/BookmarkLayoutAdaptingCard.tsx` |  | after, focus-visible, focus-within, group-focus-within, group-hover, hover | 4 | Card wrapper that adapts a bookmark's presentation to the active layout (grid, list or compact). |
| "apps/web/components/dashboard/bookmarks/BookmarkMarkdownComponent::BookmarkMarkdownComponent" | BookmarkMarkdownComponent | `apps/web/components/dashboard/bookmarks/BookmarkMarkdownComponent.tsx` |  |  | 3 | Renders a bookmark's markdown content. |
| "apps/web/components/dashboard/bookmarks/BookmarkOptions::SheetAction" | SheetAction | `apps/web/components/dashboard/bookmarks/BookmarkOptions.tsx` |  | dark, disabled, focus-visible, hover | 0 | Single action row inside the bookmark options sheet. |
| "apps/web/components/dashboard/bookmarks/BookmarkOptions::BookmarkOptionsSheet" | BookmarkOptionsSheet | `apps/web/components/dashboard/bookmarks/BookmarkOptions.tsx` |  | dark, disabled, focus-visible, hover | 0 | Sheet variant of the bookmark options menu, listing available actions. |
| "apps/web/components/dashboard/bookmarks/BookmarkOptions::BookmarkOptions" | BookmarkOptions | `apps/web/components/dashboard/bookmarks/BookmarkOptions.tsx` |  | dark, disabled, focus-visible, hover | 2 | Per-bookmark options menu exposing actions such as editing, tagging, list management and deletion. |
| "apps/web/components/dashboard/bookmarks/BookmarkOwnerIcon::BookmarkOwnerIcon" | BookmarkOwnerIcon | `apps/web/components/dashboard/bookmarks/BookmarkOwnerIcon.tsx` |  |  | 1 | Small icon indicating the owner of a bookmark. |
| "apps/web/components/dashboard/bookmarks/BookmarkTagsEditor::BookmarkTagsEditor" | BookmarkTagsEditor | `apps/web/components/dashboard/bookmarks/BookmarkTagsEditor.tsx` | variant (2) |  | 4 | Editor for the tags attached to a specific bookmark. |
| "apps/web/components/dashboard/bookmarks/BookmarkedTextEditor::BookmarkedTextEditor" | BookmarkedTextEditor | `apps/web/components/dashboard/bookmarks/BookmarkedTextEditor.tsx` |  | open | 2 | Editor for the text body of a text-type bookmark. |
| "apps/web/components/dashboard/bookmarks/Bookmarks::Bookmarks" | Bookmarks | `apps/web/components/dashboard/bookmarks/Bookmarks.tsx` |  |  | 6 | Top-level bookmarks view that loads and displays the bookmark collection. |
| "apps/web/components/dashboard/bookmarks/BookmarksGrid::StyledBookmarkCard" | StyledBookmarkCard | `apps/web/components/dashboard/bookmarks/BookmarksGrid.tsx` |  | hover | 0 | Styled card shell applied to each bookmark within the grid. |
| "apps/web/components/dashboard/bookmarks/BookmarksGrid::BookmarkGridItem" | BookmarkGridItem | `apps/web/components/dashboard/bookmarks/BookmarksGrid.tsx` |  | hover | 0 | Single item in the bookmarks grid, selecting the right card for the bookmark. |
| "apps/web/components/dashboard/bookmarks/BookmarksGrid::BookmarksGrid" | BookmarksGrid | `apps/web/components/dashboard/bookmarks/BookmarksGrid.tsx` |  | hover | 2 | Grid container laying out bookmark cards. |
| "apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton::GridCardSkeleton" | GridCardSkeleton | `apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton.tsx` |  |  | 0 | Loading placeholder shaped like a grid card. |
| "apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton::ListRowSkeleton" | ListRowSkeleton | `apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton.tsx` |  |  | 0 | Loading placeholder shaped like a list row. |
| "apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton::CompactRowSkeleton" | CompactRowSkeleton | `apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton.tsx` |  |  | 0 | Loading placeholder shaped like a compact row. |
| "apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton::BookmarksGridSkeleton" | BookmarksGridSkeleton | `apps/web/components/dashboard/bookmarks/BookmarksGridSkeleton.tsx` |  |  | 1 | Skeleton state for the whole bookmarks grid, choosing the placeholder matching the current layout. |
| "apps/web/components/dashboard/bookmarks/BulkManageListsModal::BulkManageListsModal" | BulkManageListsModal | `apps/web/components/dashboard/bookmarks/BulkManageListsModal.tsx` |  | open | 1 | Modal for adding or removing multiple selected bookmarks to and from lists. |
| "apps/web/components/dashboard/bookmarks/BulkTagModal::TagRow" | TagRow | `apps/web/components/dashboard/bookmarks/BulkTagModal.tsx` | action (2) | focus-visible, hover, open | 0 | Row representing one tag within the bulk tag modal. |
| "apps/web/components/dashboard/bookmarks/BulkTagModal::BulkTagModal" | BulkTagModal | `apps/web/components/dashboard/bookmarks/BulkTagModal.tsx` |  | focus-visible, hover, open | 1 | Modal for applying tag changes to multiple selected bookmarks at once. |
| "apps/web/components/dashboard/bookmarks/CardImage::CardImage" | CardImage | `apps/web/components/dashboard/bookmarks/CardImage.tsx` |  | dark | 3 | Image element used within bookmark cards. |
| "apps/web/components/dashboard/bookmarks/DeleteBookmarkConfirmationDialog::BulkDeleteDescription" | BulkDeleteDescription | `apps/web/components/dashboard/bookmarks/DeleteBookmarkConfirmationDialog.tsx` |  | open | 1 | Descriptive text shown when confirming deletion of multiple bookmarks. |
| "apps/web/components/dashboard/bookmarks/DeleteBookmarkConfirmationDialog::DeleteBookmarkConfirmationDialog" | DeleteBookmarkConfirmationDialog | `apps/web/components/dashboard/bookmarks/DeleteBookmarkConfirmationDialog.tsx` |  | open | 1 | Confirmation dialog shown before deleting one or more bookmarks. |
| "apps/web/components/dashboard/bookmarks/EditBookmarkDialog::EditBookmarkDialog" | EditBookmarkDialog | `apps/web/components/dashboard/bookmarks/EditBookmarkDialog.tsx` |  | open | 2 | Dialog for editing a bookmark's details. |
| "apps/web/components/dashboard/bookmarks/EditorCard::EditorCard" | EditorCard | `apps/web/components/dashboard/bookmarks/EditorCard.tsx` |  | dark, focus-visible | 1 | Card hosting the input area for creating a new bookmark. |
| "apps/web/components/dashboard/bookmarks/FooterLinkURL::FooterLinkURL" | FooterLinkURL | `apps/web/components/dashboard/bookmarks/FooterLinkURL.tsx` |  | focus-visible, hover | 4 | Footer element displaying a bookmark's link URL. |
| "apps/web/components/dashboard/bookmarks/LinkCard::LinkTitle" | LinkTitle | `apps/web/components/dashboard/bookmarks/LinkCard.tsx` |  | focus-visible | 0 | Title element for a link bookmark card. |
| "apps/web/components/dashboard/bookmarks/LinkCard::LinkImage" | LinkImage | `apps/web/components/dashboard/bookmarks/LinkCard.tsx` |  | focus-visible | 0 | Preview image for a link bookmark card. |
| "apps/web/components/dashboard/bookmarks/LinkCard::CrawlFailedIcon" | CrawlFailedIcon | `apps/web/components/dashboard/bookmarks/LinkCard.tsx` |  | focus-visible | 0 | Indicator shown when crawling a link bookmark failed. |
| "apps/web/components/dashboard/bookmarks/LinkCard::LinkCard" | LinkCard | `apps/web/components/dashboard/bookmarks/LinkCard.tsx` |  | focus-visible | 1 | Card for a link-type bookmark. |
| "apps/web/components/dashboard/bookmarks/ManageListsModal::ManageListsModal" | ManageListsModal | `apps/web/components/dashboard/bookmarks/ManageListsModal.tsx` |  | open | 0 | Modal for managing which lists a single bookmark belongs to. |
| "apps/web/components/dashboard/bookmarks/NoBookmarksBanner::NoBookmarksBanner" | NoBookmarksBanner | `apps/web/components/dashboard/bookmarks/NoBookmarksBanner.tsx` |  | dark | 1 | Empty-state banner shown when there are no bookmarks to display. |
| "apps/web/components/dashboard/bookmarks/NotePreview::NotePreview" | NotePreview | `apps/web/components/dashboard/bookmarks/NotePreview.tsx` |  | focus-visible, hover | 3 | Preview of a bookmark's note. |
| "apps/web/components/dashboard/bookmarks/SummarizeBookmarkArea::AISummary" | AISummary | `apps/web/components/dashboard/bookmarks/SummarizeBookmarkArea.tsx` |  | hover | 0 | Displays the AI-generated summary of a bookmark. |
| "apps/web/components/dashboard/bookmarks/SummarizeBookmarkArea::SummarizeBookmarkArea" | SummarizeBookmarkArea | `apps/web/components/dashboard/bookmarks/SummarizeBookmarkArea.tsx` |  | hover | 1 | Area for triggering and showing AI summarization of a bookmark. |
| "apps/web/components/dashboard/bookmarks/TagList::TagList" | TagList | `apps/web/components/dashboard/bookmarks/TagList.tsx` |  | after, hover | 7 | Displays the list of tags on a bookmark. |
| "apps/web/components/dashboard/bookmarks/TagModal::TagModal" | TagModal | `apps/web/components/dashboard/bookmarks/TagModal.tsx` |  | open | 0 | Modal for editing a single bookmark's tags. |
| "apps/web/components/dashboard/bookmarks/TagsEditor::TagsEditor" | TagsEditor | `apps/web/components/dashboard/bookmarks/TagsEditor.tsx` | variant (2), attachedBy (2) | after, dark, focus, focus-visible, focus-within, has-[>svg] | 3 | Generic tags input/editor used by the tag dialogs. |
| "apps/web/components/dashboard/bookmarks/TextCard::ClampedNote" | ClampedNote | `apps/web/components/dashboard/bookmarks/TextCard.tsx` |  | after, before, dark, focus-visible, hover | 0 | Line-clamped rendering of a text bookmark's note. |
| "apps/web/components/dashboard/bookmarks/TextCard::TextCard" | TextCard | `apps/web/components/dashboard/bookmarks/TextCard.tsx` |  | after, before, dark, focus-visible, hover | 1 | Card for a text-type bookmark. |
| "apps/web/components/dashboard/bookmarks/UnknownCard::UnknownCard" | UnknownCard | `apps/web/components/dashboard/bookmarks/UnknownCard.tsx` |  |  | 2 | Fallback card for bookmarks of an unrecognized type. |
| "apps/web/components/dashboard/bookmarks/UpdatableBookmarksGrid::UpdatableBookmarksGrid" | UpdatableBookmarksGrid | `apps/web/components/dashboard/bookmarks/UpdatableBookmarksGrid.tsx` |  |  | 1 | Grid of bookmarks in the dashboard that can refresh or update its contents in place. |
| "apps/web/components/dashboard/bookmarks/icons::SelectionCheckbox" | SelectionCheckbox | `apps/web/components/dashboard/bookmarks/icons.tsx` |  | checked, focus-visible, hover | 4 | Checkbox icon used to select a bookmark, e.g. for bulk actions. |
| "apps/web/components/dashboard/bookmarks/icons::FavouritedActionIcon" | FavouritedActionIcon | `apps/web/components/dashboard/bookmarks/icons.tsx` |  | checked, focus-visible, hover | 8 | Action icon indicating and toggling a bookmark's favourited state. |
| "apps/web/components/dashboard/bookmarks/icons::ArchivedActionIcon" | ArchivedActionIcon | `apps/web/components/dashboard/bookmarks/icons.tsx` |  | checked, focus-visible, hover | 6 | Action icon indicating and toggling a bookmark's archived state. |
| "apps/web/components/dashboard/cleanups/TagDuplicationDetention::ApplyAllButton" | ApplyAllButton | `apps/web/components/dashboard/cleanups/TagDuplicationDetention.tsx` |  | group-hover | 0 | Button that applies every pending tag-duplicate suggestion at once. |
| "apps/web/components/dashboard/cleanups/TagDuplicationDetention::SuggestionRow" | SuggestionRow | `apps/web/components/dashboard/cleanups/TagDuplicationDetention.tsx` |  | group-hover | 0 | Single row presenting one suggested tag merge within the duplication cleanup. |
| "apps/web/components/dashboard/cleanups/TagDuplicationDetention::TagDuplicationDetection" | TagDuplicationDetection | `apps/web/components/dashboard/cleanups/TagDuplicationDetention.tsx` |  | group-hover | 1 | Cleanup panel that detects duplicate tags and lists suggestions for merging them. |
| "apps/web/components/dashboard/feeds/FeedSelector::FeedSelector" | FeedSelector | `apps/web/components/dashboard/feeds/FeedSelector.tsx` |  |  | 1 | Control for choosing a feed within the dashboard feeds area. |
| "apps/web/components/dashboard/header/Header::Header" | Header | `apps/web/components/dashboard/header/Header.tsx` |  |  | 1 | Top header bar of the dashboard. |
| "apps/web/components/dashboard/header/ProfileOptions::ThemeSelector" | ThemeSelector | `apps/web/components/dashboard/header/ProfileOptions.tsx` |  | focus | 0 | Control in the profile options for switching the UI theme. |
| "apps/web/components/dashboard/header/ProfileOptions::SidebarProfileOptions" | SidebarProfileOptions | `apps/web/components/dashboard/header/ProfileOptions.tsx` |  | focus | 0 | Profile options menu rendered in the sidebar context. |
| "apps/web/components/dashboard/highlights/AllHighlights::HighlightWithTime" | HighlightWithTime | `apps/web/components/dashboard/highlights/AllHighlights.tsx` |  | dark, focus-visible, hover | 0 | A highlight entry shown together with its timestamp. |
| "apps/web/components/dashboard/highlights/AllHighlights::ArticleLink" | ArticleLink | `apps/web/components/dashboard/highlights/AllHighlights.tsx` |  | dark, focus-visible, hover | 0 | Link back to the source article a highlight belongs to. |
| "apps/web/components/dashboard/highlights/AllHighlights::ColorFilter" | ColorFilter | `apps/web/components/dashboard/highlights/AllHighlights.tsx` |  | dark, focus-visible, hover | 0 | Filter for narrowing highlights by their colour. |
| "apps/web/components/dashboard/highlights/AllHighlights::AllHighlights" | AllHighlights | `apps/web/components/dashboard/highlights/AllHighlights.tsx` |  | dark, focus-visible, hover | 1 | View listing all of the user's highlights. |
| "apps/web/components/dashboard/highlights/HighlightCard::Wrapper" | Wrapper | `apps/web/components/dashboard/highlights/HighlightCard.tsx` |  | disabled, focus-visible, group-focus-within/highlight, group-hover/highlight, hover | 0 | Layout wrapper around a highlight card. |
| "apps/web/components/dashboard/highlights/HighlightCard::HighlightCard" | HighlightCard | `apps/web/components/dashboard/highlights/HighlightCard.tsx` |  | disabled, focus-visible, group-focus-within/highlight, group-hover/highlight, hover | 5 | Card displaying a single highlight. |
| "apps/web/components/dashboard/lists/AllListsView::ListItem" | ListItem | `apps/web/components/dashboard/lists/AllListsView.tsx` |  | after, hover, last | 2 | One list entry inside the all-lists view. |
| "apps/web/components/dashboard/lists/AllListsView::Section" | Section | `apps/web/components/dashboard/lists/AllListsView.tsx` |  | after, hover, last | 4 | Grouping section within the all-lists view. |
| "apps/web/components/dashboard/lists/AllListsView::AllListsView" | AllListsView | `apps/web/components/dashboard/lists/AllListsView.tsx` |  | after, hover, last | 1 | View showing all of the user's bookmark lists. |
| "apps/web/components/dashboard/lists/BookmarkListSelector::ListSelectorComponent" | ListSelectorComponent | `apps/web/components/dashboard/lists/BookmarkListSelector.tsx` |  | dark, disabled, focus-visible, open | 0 | Underlying selector UI shared by the single and multi list selectors. |
| "apps/web/components/dashboard/lists/BookmarkListSelector::BookmarkListSingleSelector" | BookmarkListSingleSelector | `apps/web/components/dashboard/lists/BookmarkListSelector.tsx` |  | dark, disabled, focus-visible, open | 0 | Selector for picking exactly one bookmark list. |
| "apps/web/components/dashboard/lists/BookmarkListSelector::BookmarkListMultiSelector" | BookmarkListMultiSelector | `apps/web/components/dashboard/lists/BookmarkListSelector.tsx` |  | dark, disabled, focus-visible, open | 0 | Selector for picking multiple bookmark lists. |
| "apps/web/components/dashboard/lists/BookmarkListSelector::BookmarkListSelector" | BookmarkListSelector | `apps/web/components/dashboard/lists/BookmarkListSelector.tsx` |  | dark, disabled, focus-visible, open | 5 | Entry-point selector component for choosing bookmark lists. |
| "apps/web/components/dashboard/lists/CollapsibleBookmarkLists::ListItem" | ListItem | `apps/web/components/dashboard/lists/CollapsibleBookmarkLists.tsx` |  | open | 4 | One list entry inside the collapsible lists tree. |
| "apps/web/components/dashboard/lists/CollapsibleBookmarkLists::CollapsibleBookmarkLists" | CollapsibleBookmarkLists | `apps/web/components/dashboard/lists/CollapsibleBookmarkLists.tsx` |  | open | 4 | Collapsible, expandable presentation of bookmark lists. |
| "apps/web/components/dashboard/lists/DeleteListConfirmationDialog::DeleteListConfirmationDialog" | DeleteListConfirmationDialog | `apps/web/components/dashboard/lists/DeleteListConfirmationDialog.tsx` |  | open | 1 | Confirmation dialog shown before deleting a list. |
| "apps/web/components/dashboard/lists/EditListModal::EditListModal" | EditListModal | `apps/web/components/dashboard/lists/EditListModal.tsx` |  | group-data-[state=open], hover, open | 7 | Modal for creating or editing a list's details. |
| "apps/web/components/dashboard/lists/LeaveListConfirmationDialog::LeaveListConfirmationDialog" | LeaveListConfirmationDialog | `apps/web/components/dashboard/lists/LeaveListConfirmationDialog.tsx` |  | open | 1 | Confirmation dialog shown before leaving a shared list. |
| "apps/web/components/dashboard/lists/ListHeader::ListHeader" | ListHeader | `apps/web/components/dashboard/lists/ListHeader.tsx` |  | hover | 1 | Header shown at the top of a list page. |
| "apps/web/components/dashboard/lists/ListHeaderComponents::ListPrivacyLabel" | ListPrivacyLabel | `apps/web/components/dashboard/lists/ListHeaderComponents.tsx` |  | group-hover | 3 | Label indicating a list's privacy setting. |
| "apps/web/components/dashboard/lists/ListHeaderComponents::ListCollaboratorsIcons" | ListCollaboratorsIcons | `apps/web/components/dashboard/lists/ListHeaderComponents.tsx` |  | group-hover | 2 | Row of icons representing a list's collaborators. |
| "apps/web/components/dashboard/lists/ListHeaderComponents::ListItemCount" | ListItemCount | `apps/web/components/dashboard/lists/ListHeaderComponents.tsx` |  | group-hover | 2 | Count of items contained in a list. |
| "apps/web/components/dashboard/lists/ListNamePicker::ListNamePicker" | ListNamePicker | `apps/web/components/dashboard/lists/ListNamePicker.tsx` |  | placeholder | 1 | Input for choosing a list's name. |
| "apps/web/components/dashboard/lists/ListOptions::ListOptions" | ListOptions | `apps/web/components/dashboard/lists/ListOptions.tsx` |  | disabled | 3 | Options menu with actions available for a list. |
| "apps/web/components/dashboard/lists/ManageCollaboratorsModal::ManageCollaboratorsModal" | ManageCollaboratorsModal | `apps/web/components/dashboard/lists/ManageCollaboratorsModal.tsx` |  | hover, open | 1 | Modal for managing who collaborates on a list. |
| "apps/web/components/dashboard/lists/MergeListModal::MergeListModal" | MergeListModal | `apps/web/components/dashboard/lists/MergeListModal.tsx` |  | open | 1 | Modal for merging one list into another. |
| "apps/web/components/dashboard/lists/NewListButton::NewListButton" | NewListButton | `apps/web/components/dashboard/lists/NewListButton.tsx` |  |  | 1 | Button that starts creation of a new list. |
| "apps/web/components/dashboard/lists/PendingInvitationsCard::InvitationRow" | InvitationRow | `apps/web/components/dashboard/lists/PendingInvitationsCard.tsx` |  |  | 1 | Single pending list invitation within the invitations card. |
| "apps/web/components/dashboard/lists/PendingInvitationsCard::PendingInvitationsCard" | PendingInvitationsCard | `apps/web/components/dashboard/lists/PendingInvitationsCard.tsx` |  |  | 1 | Card listing pending invitations to shared lists. |
| "apps/web/components/dashboard/lists/PublicListLink::PublicListLink" | PublicListLink | `apps/web/components/dashboard/lists/PublicListLink.tsx` |  |  | 1 | Displays the public URL for a shared list so it can be viewed or copied. |
| "apps/web/components/dashboard/lists/RssLink::RssLink" | RssLink | `apps/web/components/dashboard/lists/RssLink.tsx` |  |  | 1 | Exposes the RSS feed link for a list. |
| "apps/web/components/dashboard/lists/ShareListModal::ShareListModal" | ShareListModal | `apps/web/components/dashboard/lists/ShareListModal.tsx` |  | open | 1 | Modal dialog for sharing a list, housing controls such as @apps/web/components/dashboard/lists/PublicListLink::PublicListLink and @apps/web/components/dashboard/lists/RssLink::RssLink. |
| "apps/web/components/dashboard/lists/SmartListPreview::SmartListPreview" | SmartListPreview | `apps/web/components/dashboard/lists/SmartListPreview.tsx` |  |  | 1 | Shows a preview of the bookmarks a smart list's query would match. |
| "apps/web/components/dashboard/lists/SmartListQueryBuilder::SmartListQueryBuilder" | SmartListQueryBuilder | `apps/web/components/dashboard/lists/SmartListQueryBuilder.tsx` |  | after, hover | 1 | Editor for composing the query that defines a smart list. |
| "apps/web/components/dashboard/preview/ActionBar::ActionBar" | ActionBar | `apps/web/components/dashboard/preview/ActionBar.tsx` |  |  | 4 | Row of actions available on the bookmark preview. |
| "apps/web/components/dashboard/preview/ArticleTitleBlock::ArticleTitleBlock" | ArticleTitleBlock | `apps/web/components/dashboard/preview/ArticleTitleBlock.tsx` |  | focus-visible, hover | 3 | Title header block for an article shown in the reader. |
| "apps/web/components/dashboard/preview/AssetContentSection::PDFContentSection" | PDFContentSection | `apps/web/components/dashboard/preview/AssetContentSection.tsx` |  |  | 0 | Renders the content of a PDF asset bookmark. |
| "apps/web/components/dashboard/preview/AssetContentSection::ImageContentSection" | ImageContentSection | `apps/web/components/dashboard/preview/AssetContentSection.tsx` |  |  | 0 | Renders the content of an image asset bookmark. |
| "apps/web/components/dashboard/preview/AssetContentSection::AssetContentSection" | AssetContentSection | `apps/web/components/dashboard/preview/AssetContentSection.tsx` |  |  | 1 | Chooses the appropriate asset renderer (@apps/web/components/dashboard/preview/AssetContentSection::PDFContentSection or @apps/web/components/dashboard/preview/AssetContentSection::ImageContentSection) for an asset bookmark. |
| "apps/web/components/dashboard/preview/AttachmentBox::EmptyActionSlot" | EmptyActionSlot | `apps/web/components/dashboard/preview/AttachmentBox.tsx` |  | hover | 0 | Placeholder slot shown where an attachment action would otherwise appear. |
| "apps/web/components/dashboard/preview/AttachmentBox::AttachmentBox" | AttachmentBox | `apps/web/components/dashboard/preview/AttachmentBox.tsx` |  | hover | 2 | Panel listing a bookmark's attachments and their actions. |
| "apps/web/components/dashboard/preview/BookmarkListsField::BookmarkListsField" | BookmarkListsField | `apps/web/components/dashboard/preview/BookmarkListsField.tsx` |  | after, focus-visible, hover | 1 | Field showing and editing which lists a bookmark belongs to. |
| "apps/web/components/dashboard/preview/BookmarkLoadError::BookmarkLoadError" | BookmarkLoadError | `apps/web/components/dashboard/preview/BookmarkLoadError.tsx` |  |  | 3 | Error state displayed when a bookmark fails to load. |
| "apps/web/components/dashboard/preview/BookmarkPreview::ContentLoading" | ContentLoading | `apps/web/components/dashboard/preview/BookmarkPreview.tsx` |  | dark, data-[state=active], data-[state=inactive], empty, hover | 0 | Loading state shown while bookmark content is being fetched. |
| "apps/web/components/dashboard/preview/BookmarkPreview::MetadataDate" | MetadataDate | `apps/web/components/dashboard/preview/BookmarkPreview.tsx` |  | dark, data-[state=active], data-[state=inactive], empty, hover | 0 | Formats a date entry within the bookmark metadata. |
| "apps/web/components/dashboard/preview/BookmarkPreview::ArchivedStatus" | ArchivedStatus | `apps/web/components/dashboard/preview/BookmarkPreview.tsx` |  | dark, data-[state=active], data-[state=inactive], empty, hover | 0 | Indicates whether the bookmark is archived. |
| "apps/web/components/dashboard/preview/BookmarkPreview::SavedDate" | SavedDate | `apps/web/components/dashboard/preview/BookmarkPreview.tsx` |  | dark, data-[state=active], data-[state=inactive], empty, hover | 0 | Shows when the bookmark was saved. |
| "apps/web/components/dashboard/preview/BookmarkPreview::LinkMetadata" | LinkMetadata | `apps/web/components/dashboard/preview/BookmarkPreview.tsx` |  | dark, data-[state=active], data-[state=inactive], empty, hover | 0 | Metadata summary for a link bookmark. |
| "apps/web/components/dashboard/preview/BookmarkPreview::DetailsTitle" | DetailsTitle | `apps/web/components/dashboard/preview/BookmarkPreview.tsx` |  | dark, data-[state=active], data-[state=inactive], empty, hover | 0 | Title shown in the bookmark details area. |
| "apps/web/components/dashboard/preview/BookmarkPreview::LinkDetailsTitle" | LinkDetailsTitle | `apps/web/components/dashboard/preview/BookmarkPreview.tsx` |  | dark, data-[state=active], data-[state=inactive], empty, hover | 0 | Link-specific variant of the details title. |
| "apps/web/components/dashboard/preview/BookmarkPreview::ViewOriginalButton" | ViewOriginalButton | `apps/web/components/dashboard/preview/BookmarkPreview.tsx` |  | dark, data-[state=active], data-[state=inactive], empty, hover | 0 | Button that opens the original source of the bookmark. |
| "apps/web/components/dashboard/preview/BookmarkPreview::NavigationButtons" | NavigationButtons | `apps/web/components/dashboard/preview/BookmarkPreview.tsx` |  | dark, data-[state=active], data-[state=inactive], empty, hover | 0 | Controls for moving to the previous or next bookmark in the preview. |
| "apps/web/components/dashboard/preview/BookmarkPreview::CloseButton" | CloseButton | `apps/web/components/dashboard/preview/BookmarkPreview.tsx` |  | dark, data-[state=active], data-[state=inactive], empty, hover | 0 | Closes the bookmark preview. |
| "apps/web/components/dashboard/preview/BookmarkPreview::BookmarkPreview" | BookmarkPreview | `apps/web/components/dashboard/preview/BookmarkPreview.tsx` |  | dark, data-[state=active], data-[state=inactive], empty, hover | 2 | Container for the full bookmark preview, composing content, metadata, navigation and actions. |
| "apps/web/components/dashboard/preview/HighlightsBox::HighlightsBox" | HighlightsBox | `apps/web/components/dashboard/preview/HighlightsBox.tsx` |  | focus-visible, hover | 1 | Panel listing the highlights made on a bookmark. |
| "apps/web/components/dashboard/preview/IconControl::IconTooltip" | IconTooltip | `apps/web/components/dashboard/preview/IconControl.tsx` | side (4) | hover | 29 | Tooltip wrapper for an icon control in the preview. |
| "apps/web/components/dashboard/preview/IconControl::RestoreTooltip" | RestoreTooltip | `apps/web/components/dashboard/preview/IconControl.tsx` |  | hover | 2 | Tooltip for a restore icon control. |
| "apps/web/components/dashboard/preview/LinkContentSection::CustomRendererErrorFallback" | CustomRendererErrorFallback | `apps/web/components/dashboard/preview/LinkContentSection.tsx` |  |  | 0 | Fallback shown when a custom content renderer errors. |
| "apps/web/components/dashboard/preview/LinkContentSection::FullPageArchiveSection" | FullPageArchiveSection | `apps/web/components/dashboard/preview/LinkContentSection.tsx` |  |  | 0 | Displays the full-page archive of a link. |
| "apps/web/components/dashboard/preview/LinkContentSection::ScreenshotSection" | ScreenshotSection | `apps/web/components/dashboard/preview/LinkContentSection.tsx` |  |  | 0 | Displays the stored screenshot of a link. |
| "apps/web/components/dashboard/preview/LinkContentSection::VideoSection" | VideoSection | `apps/web/components/dashboard/preview/LinkContentSection.tsx` |  |  | 0 | Displays video content for a link. |
| "apps/web/components/dashboard/preview/LinkContentSection::PDFSection" | PDFSection | `apps/web/components/dashboard/preview/LinkContentSection.tsx` |  |  | 0 | Displays PDF content for a link. |
| "apps/web/components/dashboard/preview/LinkContentSection::LinkContentSection" | LinkContentSection | `apps/web/components/dashboard/preview/LinkContentSection.tsx` |  |  | 1 | Selects and renders the chosen view of a link bookmark's content, delegating to the archive, screenshot, video or PDF sections. |
| "apps/web/components/dashboard/preview/LinkViewMenu::LinkViewMenu" | LinkViewMenu | `apps/web/components/dashboard/preview/LinkViewMenu.tsx` |  |  | 1 | Menu for switching between available views of a link's content. |
| "apps/web/components/dashboard/preview/NoteEditor::NoteEditor" | NoteEditor | `apps/web/components/dashboard/preview/NoteEditor.tsx` |  | dark, placeholder | 2 | Editor for the note attached to a bookmark. |
| "apps/web/components/dashboard/preview/ReaderBarActions::TagsPopoverContent" | TagsPopoverContent | `apps/web/components/dashboard/preview/ReaderBarActions.tsx` |  |  | 0 | Popover content for viewing and editing a bookmark's tags from the reader bar. |
| "apps/web/components/dashboard/preview/ReaderBarActions::ReaderBarActions" | ReaderBarActions | `apps/web/components/dashboard/preview/ReaderBarActions.tsx` |  |  | 1 | Action group in the reader bar, including tags and an overflow menu. |
| "apps/web/components/dashboard/preview/ReaderBarActions::ReaderMoreMenu" | ReaderMoreMenu | `apps/web/components/dashboard/preview/ReaderBarActions.tsx` |  |  | 1 | Overflow menu of additional reader actions. |
| "apps/web/components/dashboard/preview/ReaderSettingsPopover::ReaderSettingsPopover" | ReaderSettingsPopover | `apps/web/components/dashboard/preview/ReaderSettingsPopover.tsx` | variant (2) | after, dark, hover | 2 | Popover for adjusting reader display settings. |
| "apps/web/components/dashboard/preview/ReaderView::ReaderView" | ReaderView | `apps/web/components/dashboard/preview/ReaderView.tsx` |  |  | 2 | Reader-oriented presentation of a saved page's content within the dashboard preview. |
| "apps/web/components/dashboard/preview/ReadingProgressBanner::ReadingProgressBanner" | ReadingProgressBanner | `apps/web/components/dashboard/preview/ReadingProgressBanner.tsx` |  | hover | 1 | Banner in the preview that surfaces reading progress for a saved page. |
| "apps/web/components/dashboard/preview/SavedPageOverview::Favicon" | Favicon | `apps/web/components/dashboard/preview/SavedPageOverview.tsx` |  |  | 0 | Favicon display used within the saved-page overview. |
| "apps/web/components/dashboard/preview/SavedPageOverview::SavedPageOverview" | SavedPageOverview | `apps/web/components/dashboard/preview/SavedPageOverview.tsx` |  |  | 1 | Summary view of a saved page shown in the dashboard preview. |
| "apps/web/components/dashboard/preview/TextContentSection::TextContentSection" | TextContentSection | `apps/web/components/dashboard/preview/TextContentSection.tsx` |  | hover | 1 | Section of the preview that renders a saved item's text content. |
| "apps/web/components/dashboard/preview/UnavailableViewOption::UnavailableViewOption" | UnavailableViewOption | `apps/web/components/dashboard/preview/UnavailableViewOption.tsx` |  | data-[disabled] | 1 | Placeholder shown when a preview view option is not available for the item. |
| "apps/web/components/dashboard/preview/content-renderers/AmazonRenderer::AmazonRendererComponent" | AmazonRendererComponent | `apps/web/components/dashboard/preview/content-renderers/AmazonRenderer.tsx` |  | hover | 0 | Content renderer for saved Amazon pages in the preview. |
| "apps/web/components/dashboard/preview/content-renderers/InstagramRenderer::InstagramRendererComponent" | InstagramRendererComponent | `apps/web/components/dashboard/preview/content-renderers/InstagramRenderer.tsx` |  |  | 0 | Content renderer for saved Instagram content in the preview. |
| "apps/web/components/dashboard/preview/content-renderers/TikTokRenderer::TikTokRendererComponent" | TikTokRendererComponent | `apps/web/components/dashboard/preview/content-renderers/TikTokRenderer.tsx` |  |  | 0 | Content renderer for saved TikTok content in the preview. |
| "apps/web/components/dashboard/preview/content-renderers/XRenderer::XRendererComponent" | XRendererComponent | `apps/web/components/dashboard/preview/content-renderers/XRenderer.tsx` |  |  | 0 | Content renderer for saved X posts in the preview. |
| "apps/web/components/dashboard/preview/content-renderers/YouTubeRenderer::YouTubeRendererComponent" | YouTubeRendererComponent | `apps/web/components/dashboard/preview/content-renderers/YouTubeRenderer.tsx` |  |  | 0 | Content renderer for saved YouTube content in the preview. |
| "apps/web/components/dashboard/rules/RuleEngineActionBuilder::ActionBuilder" | ActionBuilder | `apps/web/components/dashboard/rules/RuleEngineActionBuilder.tsx` |  | dark, has-[>svg], hover | 1 | Builder for the actions a rule performs in the rules engine. |
| "apps/web/components/dashboard/rules/RuleEngineConditionBuilder::ConditionBuilder" | ConditionBuilder | `apps/web/components/dashboard/rules/RuleEngineConditionBuilder.tsx` |  | dark, has-[>svg], hover | 1 | Builder for the conditions a rule evaluates in the rules engine. |
| "apps/web/components/dashboard/rules/RuleEngineEventSelector::EventSelector" | EventSelector | `apps/web/components/dashboard/rules/RuleEngineEventSelector.tsx` |  |  | 1 | Selector for the triggering event of a rule. |
| "apps/web/components/dashboard/rules/RuleEngineRuleEditor::RuleEditor" | RuleEditor | `apps/web/components/dashboard/rules/RuleEngineRuleEditor.tsx` |  |  | 1 | Editor composing event, conditions, and actions into a single rule. |
| "apps/web/components/dashboard/rules/RuleEngineRuleList::RuleList" | RuleList | `apps/web/components/dashboard/rules/RuleEngineRuleList.tsx` |  |  | 1 | List of existing rules in the rules engine. |
| "apps/web/components/dashboard/search/QueryExplainerTooltip::MatcherComp" | MatcherComp | `apps/web/components/dashboard/search/QueryExplainerTooltip.tsx` |  |  | 0 | Displays an individual matcher inside the query explainer tooltip. |
| "apps/web/components/dashboard/search/QueryExplainerTooltip::QueryExplainerTooltip" | QueryExplainerTooltip | `apps/web/components/dashboard/search/QueryExplainerTooltip.tsx` |  |  | 3 | Tooltip explaining how a search query is interpreted. |
| "apps/web/components/dashboard/search/SearchInput::SearchInput" | SearchInput | `apps/web/components/dashboard/search/SearchInput.tsx` |  | hover | 4 | Text input for searching saved items in the dashboard. |
| "apps/web/components/dashboard/search/SearchModeSelector::SearchModeSelector" | SearchModeSelector | `apps/web/components/dashboard/search/SearchModeSelector.tsx` |  | group-data-[state=open], hover | 3 | Control for choosing the search mode. |
| "apps/web/components/dashboard/sidebar/AllLists::DroppableListSidebarItem" | DroppableListSidebarItem | `apps/web/components/dashboard/sidebar/AllLists.tsx` |  | group-hover, open | 0 | Sidebar list item that accepts dropped items. |
| "apps/web/components/dashboard/sidebar/AllLists::AllLists" | AllLists | `apps/web/components/dashboard/sidebar/AllLists.tsx` |  | group-hover, open | 1 | Sidebar section listing all of the user's lists. |
| "apps/web/components/dashboard/sidebar/InvitationNotificationBadge::InvitationNotificationBadge" | InvitationNotificationBadge | `apps/web/components/dashboard/sidebar/InvitationNotificationBadge.tsx` |  |  | 1 | Badge in the sidebar indicating pending invitations. |
| "apps/web/components/dashboard/tags/AllTagsView::DeleteAllUnusedTags" | DeleteAllUnusedTags | `apps/web/components/dashboard/tags/AllTagsView.tsx` |  |  | 0 | Action for deleting all tags that are not in use. |
| "apps/web/components/dashboard/tags/AllTagsView::AllTagsView" | AllTagsView | `apps/web/components/dashboard/tags/AllTagsView.tsx` |  |  | 1 | View listing all tags in the dashboard. |
| "apps/web/components/dashboard/tags/BulkTagAction::BulkTagAction" | BulkTagAction | `apps/web/components/dashboard/tags/BulkTagAction.tsx` |  |  | 1 | Applies a tag action to multiple items at once. |
| "apps/web/components/dashboard/tags/CreateTagModal::CreateTagModal" | CreateTagModal | `apps/web/components/dashboard/tags/CreateTagModal.tsx` |  |  | 1 | Modal for creating a new tag. |
| "apps/web/components/dashboard/tags/DeleteTagConfirmationDialog::DeleteTagConfirmationDialog" | DeleteTagConfirmationDialog | `apps/web/components/dashboard/tags/DeleteTagConfirmationDialog.tsx` |  |  | 2 | Confirmation dialog before deleting a tag. |
| "apps/web/components/dashboard/tags/EditableTagName::EditableTagName" | EditableTagName | `apps/web/components/dashboard/tags/EditableTagName.tsx` |  |  | 0 | Inline-editable tag name. |
| "apps/web/components/dashboard/tags/MergeTagModal::MergeTagModal" | MergeTagModal | `apps/web/components/dashboard/tags/MergeTagModal.tsx` |  | open | 1 | Modal for merging one tag into another. |
| "apps/web/components/dashboard/tags/MultiTagSelector::MultiTagSelector" | MultiTagSelector | `apps/web/components/dashboard/tags/MultiTagSelector.tsx` |  | dark, group-hover, hover | 1 | Selector for choosing multiple tags. |
| "apps/web/components/dashboard/tags/RenameTagModal::RenameTagModal" | RenameTagModal | `apps/web/components/dashboard/tags/RenameTagModal.tsx` |  | open | 1 | Modal for renaming a tag. |
| "apps/web/components/dashboard/tags/TagAutocomplete::TagAutocomplete" | TagAutocomplete | `apps/web/components/dashboard/tags/TagAutocomplete.tsx` |  | hover, placeholder | 4 | Autocomplete input for finding and selecting tags. |
| "apps/web/components/dashboard/tags/TagAutocomplete::TagNamePicker" | TagNamePicker | `apps/web/components/dashboard/tags/TagAutocomplete.tsx` |  | hover, placeholder | 1 | Picker for a tag name, built on the tag autocomplete. |
| "apps/web/components/dashboard/tags/TagHeader::TagHeader" | TagHeader | `apps/web/components/dashboard/tags/TagHeader.tsx` |  |  | 1 | Header for a tag's page in the dashboard. |
| "apps/web/components/dashboard/tags/TagOptions::TagOptions" | TagOptions | `apps/web/components/dashboard/tags/TagOptions.tsx` |  |  | 1 | Options menu for actions on a tag. |
| "apps/web/components/dashboard/tags/TagPill::TagPill" | TagPill | `apps/web/components/dashboard/tags/TagPill.tsx` |  | dark, group-hover, hover | 4 | Pill-shaped tag label used in the dashboard. |
| "apps/web/components/invite/InviteAcceptForm::InviteAcceptForm" | InviteAcceptForm | `apps/web/components/invite/InviteAcceptForm.tsx` |  |  | 1 | Form for accepting an invitation. |
| "apps/web/components/public/lists/PublicBookmarkGrid::TagPill" | TagPill | `apps/web/components/public/lists/PublicBookmarkGrid.tsx` |  | dark, focus-visible, group-hover, hover | 3 | Pill-shaped tag label used in the public bookmark grid. |
| "apps/web/components/public/lists/PublicBookmarkGrid::PublicCardImage" | PublicCardImage | `apps/web/components/public/lists/PublicBookmarkGrid.tsx` |  | dark, focus-visible, group-hover, hover | 0 | Image for a bookmark card in the public list grid. |
| "apps/web/components/public/lists/PublicBookmarkGrid::ExpandNote" | ExpandNote | `apps/web/components/public/lists/PublicBookmarkGrid.tsx` |  | dark, focus-visible, group-hover, hover | 0 | Control within the public bookmark grid for expanding a bookmark's note. |
| "apps/web/components/public/lists/PublicBookmarkGrid::BookmarkCard" | BookmarkCard | `apps/web/components/public/lists/PublicBookmarkGrid.tsx` |  | dark, focus-visible, group-hover, hover | 3 | Card representing a single bookmark inside a public list grid. |
| "apps/web/components/public/lists/PublicBookmarkGrid::PublicBookmarkGrid" | PublicBookmarkGrid | `apps/web/components/public/lists/PublicBookmarkGrid.tsx` |  | dark, focus-visible, group-hover, hover | 1 | Grid layout that displays the bookmarks of a publicly shared list. |
| "apps/web/components/public/lists/PublicListHeader::PublicListHeader" | PublicListHeader | `apps/web/components/public/lists/PublicListHeader.tsx` |  | focus-visible, hover | 1 | Header shown at the top of a publicly shared list page. |
| "apps/web/components/settings/AISettings::AIPreferences" | AIPreferences | `apps/web/components/settings/AISettings.tsx` |  | dark, hover | 0 | Section of AI settings for the user's AI-related preferences. |
| "apps/web/components/settings/AISettings::TagStyleSelector" | TagStyleSelector | `apps/web/components/settings/AISettings.tsx` |  | dark, hover | 0 | Selector for choosing the style of AI-generated tags. |
| "apps/web/components/settings/AISettings::CuratedTagsSelector" | CuratedTagsSelector | `apps/web/components/settings/AISettings.tsx` |  | dark, hover | 0 | Selector for managing a curated set of tags used by AI tagging. |
| "apps/web/components/settings/AISettings::PromptEditor" | PromptEditor | `apps/web/components/settings/AISettings.tsx` |  | dark, hover | 0 | Editor for authoring a custom AI prompt. |
| "apps/web/components/settings/AISettings::PromptRow" | PromptRow | `apps/web/components/settings/AISettings.tsx` |  | dark, hover | 0 | Single row representing one saved prompt in the AI settings list. |
| "apps/web/components/settings/AISettings::TaggingRules" | TaggingRules | `apps/web/components/settings/AISettings.tsx` |  | dark, hover | 0 | Section for configuring rules that govern AI tagging. |
| "apps/web/components/settings/AISettings::PromptDemo" | PromptDemo | `apps/web/components/settings/AISettings.tsx` |  | dark, hover | 0 | Demonstration area showing how a prompt behaves. |
| "apps/web/components/settings/AISettings::AISettings" | AISettings | `apps/web/components/settings/AISettings.tsx` |  | dark, hover | 1 | Top-level AI settings page composing preferences, tag selectors, prompts and tagging rules. |
| "apps/web/components/settings/AddApiKey::ScopeCard" | ScopeCard | `apps/web/components/settings/AddApiKey.tsx` |  | disabled, has-[[data-state=checked]], hover | 0 | Card grouping scope options when creating an API key. |
| "apps/web/components/settings/AddApiKey::ScopeChoiceRow" | ScopeChoiceRow | `apps/web/components/settings/AddApiKey.tsx` |  | disabled, has-[[data-state=checked]], hover | 0 | Row for selecting an individual scope choice for an API key. |
| "apps/web/components/settings/AddApiKey::AddApiKeyForm" | AddApiKeyForm | `apps/web/components/settings/AddApiKey.tsx` |  | disabled, has-[[data-state=checked]], hover | 0 | Form collecting the details needed to create a new API key. |
| "apps/web/components/settings/AddApiKey::AddApiKey" | AddApiKey | `apps/web/components/settings/AddApiKey.tsx` |  | disabled, has-[[data-state=checked]], hover | 2 | Entry point that wraps the add-API-key flow. |
| "apps/web/components/settings/ApiKeyRowActions::ApiKeyRowActions" | ApiKeyRowActions | `apps/web/components/settings/ApiKeyRowActions.tsx` |  |  | 1 | Action controls attached to a single API key row. |
| "apps/web/components/settings/ApiKeySettings::ApiKeys" | ApiKeys | `apps/web/components/settings/ApiKeySettings.tsx` |  |  | 0 | Settings view listing the user's API keys. |
| "apps/web/components/settings/ApiKeySuccess::ApiKeySuccess" | ApiKeySuccess | `apps/web/components/settings/ApiKeySuccess.tsx` |  |  | 2 | Confirmation state shown after an API key is successfully created. |
| "apps/web/components/settings/BackupSettings::BackupConfigurationForm" | BackupConfigurationForm | `apps/web/components/settings/BackupSettings.tsx` |  | disabled | 0 | Form for configuring backup options. |
| "apps/web/components/settings/BackupSettings::BackupRow" | BackupRow | `apps/web/components/settings/BackupSettings.tsx` |  | disabled | 0 | Row representing a single backup in the backups list. |
| "apps/web/components/settings/BackupSettings::BackupsList" | BackupsList | `apps/web/components/settings/BackupSettings.tsx` |  | disabled | 0 | List of existing backups. |
| "apps/web/components/settings/BackupSettings::BackupSettings" | BackupSettings | `apps/web/components/settings/BackupSettings.tsx` |  | disabled | 1 | Top-level backup settings page combining configuration and the backups list. |
| "apps/web/components/settings/ChangePassword::ChangePassword" | ChangePassword | `apps/web/components/settings/ChangePassword.tsx` |  |  | 1 | Settings form for changing the account password. |
| "apps/web/components/settings/DeleteAccount::DeleteAccount" | DeleteAccount | `apps/web/components/settings/DeleteAccount.tsx` |  |  | 1 | Settings control for deleting the user's account. |
| "apps/web/components/settings/DeleteApiKey::DeleteApiKey" | DeleteApiKey | `apps/web/components/settings/DeleteApiKey.tsx` |  | open | 1 | Control for deleting an API key. |
| "apps/web/components/settings/FeedSettings::FeedsEditorDialog" | FeedsEditorDialog | `apps/web/components/settings/FeedSettings.tsx` |  | disabled, hover, open | 0 | Dialog for editing feeds. |
| "apps/web/components/settings/FeedSettings::EditFeedDialog" | EditFeedDialog | `apps/web/components/settings/FeedSettings.tsx` |  | disabled, hover, open | 0 | Dialog for editing a single feed. |
| "apps/web/components/settings/FeedSettings::FeedRow" | FeedRow | `apps/web/components/settings/FeedSettings.tsx` |  | disabled, hover, open | 0 | Row representing one feed in the feed settings list. |
| "apps/web/components/settings/FeedSettings::FeedSettings" | FeedSettings | `apps/web/components/settings/FeedSettings.tsx` |  | disabled, hover, open | 1 | Top-level feed settings page listing feeds and their editors. |
| "apps/web/components/settings/ImportExport::ExportSection" | ExportSection | `apps/web/components/settings/ImportExport.tsx` |  | focus-visible, hover | 0 | Section of import/export settings handling data export. |
| "apps/web/components/settings/ImportExport::ImportProviderRow" | ImportProviderRow | `apps/web/components/settings/ImportExport.tsx` |  | focus-visible, hover | 0 | Row for a single import provider option. |
| "apps/web/components/settings/ImportExport::ImportSection" | ImportSection | `apps/web/components/settings/ImportExport.tsx` |  | focus-visible, hover | 0 | Section of import/export settings handling data import. |
| "apps/web/components/settings/ImportExport::ImportExport" | ImportExport | `apps/web/components/settings/ImportExport.tsx` |  | focus-visible, hover | 1 | Top-level import/export settings page composing the import and export sections. |
| "apps/web/components/settings/ImportSessionCard::ImportSessionCard" | ImportSessionCard | `apps/web/components/settings/ImportSessionCard.tsx` |  | dark, hover | 1 | Card summarizing a single import session. |
| "apps/web/components/settings/ImportSessionDetail::ImportSessionDetail" | ImportSessionDetail | `apps/web/components/settings/ImportSessionDetail.tsx` |  | dark, hover | 1 | Detailed view of one import session. |
| "apps/web/components/settings/ImportSessionsSection::ImportSessionsSection" | ImportSessionsSection | `apps/web/components/settings/ImportSessionsSection.tsx` |  |  | 1 | Section listing import sessions. |
| "apps/web/components/settings/Maintenance::SelectionCheckbox" | SelectionCheckbox | `apps/web/components/settings/Maintenance.tsx` |  | after, disabled | 4 | Checkbox used to select items within the maintenance view. |
| "apps/web/components/settings/Maintenance::MaintenanceSearch" | MaintenanceSearch | `apps/web/components/settings/Maintenance.tsx` |  | after, disabled | 1 | Search control within the maintenance settings. |
| "apps/web/components/settings/Maintenance::MaintenanceError" | MaintenanceError | `apps/web/components/settings/Maintenance.tsx` |  | after, disabled | 1 | Error display used within the maintenance settings. |
| "apps/web/components/settings/ProfileNameForm::ProfileNameForm" | ProfileNameForm | `apps/web/components/settings/ProfileNameForm.tsx` |  |  | 1 | Settings form for editing the user's profile name. |
| "apps/web/components/settings/ReadingSettings::ReadingSettings" | ReadingSettings | `apps/web/components/settings/ReadingSettings.tsx` | key (3) |  | 1 | Settings section for reading-related preferences. |
| "apps/web/components/settings/RegenerateApiKey::RegenerateApiKey" | RegenerateApiKey | `apps/web/components/settings/RegenerateApiKey.tsx` |  | open | 1 | Control for regenerating the user's API key. |
| "apps/web/components/settings/RowActions::RowIconButton" | RowIconButton | `apps/web/components/settings/RowActions.tsx` |  | dark, disabled, focus-visible, hover | 1 | Icon-only button used for actions within a settings row. |
| "apps/web/components/settings/RowActions::RowActionsMenu" | RowActionsMenu | `apps/web/components/settings/RowActions.tsx` |  | dark, disabled, focus-visible, hover | 6 | Menu grouping multiple actions for a settings row. |
| "apps/web/components/settings/SaveBar::SaveBar" | SaveBar | `apps/web/components/settings/SaveBar.tsx` |  | motion-reduce | 2 | Bar exposing save controls for pending settings changes. |
| "apps/web/components/settings/SavedHint::SavedHint" | SavedHint | `apps/web/components/settings/SavedHint.tsx` |  |  | 9 | Inline hint confirming that settings were saved. |
| "apps/web/components/settings/SectionNav::SectionMobileBar" | SectionMobileBar | `apps/web/components/settings/SectionNav.tsx` |  | focus-visible, hover | 2 | Mobile-width navigation bar for moving between settings sections. |
| "apps/web/components/settings/SectionNav::SectionIndex" | SectionIndex | `apps/web/components/settings/SectionNav.tsx` |  | focus-visible, hover | 2 | Index listing of settings sections for navigation. |
| "apps/web/components/settings/SectionSidebar::SectionSidebar" | SectionSidebar | `apps/web/components/settings/SectionSidebar.tsx` |  |  | 2 | Sidebar navigation for settings sections. |
| "apps/web/components/settings/SettingsPage::SettingsPage" | SettingsPage | `apps/web/components/settings/SettingsPage.tsx` |  | has-[[data-save-bar]] | 19 | Top-level layout wrapper for a settings page. |
| "apps/web/components/settings/SettingsPage::SettingsSection" | SettingsSection | `apps/web/components/settings/SettingsPage.tsx` |  | has-[[data-save-bar]] | 35 | Titled section container within a settings page. |
| "apps/web/components/settings/SettingsPage::SettingsRow" | SettingsRow | `apps/web/components/settings/SettingsPage.tsx` |  | has-[[data-save-bar]] | 27 | Single labeled row within a settings section. |
| "apps/web/components/settings/SettingsPage::SettingsRows" | SettingsRows | `apps/web/components/settings/SettingsPage.tsx` |  | has-[[data-save-bar]] | 6 | Container grouping a list of settings rows. |
| "apps/web/components/settings/SettingsPage::SettingsFormFooter" | SettingsFormFooter | `apps/web/components/settings/SettingsPage.tsx` |  | has-[[data-save-bar]] | 2 | Footer area for a settings form's actions. |
| "apps/web/components/settings/SubscriptionSettings::SubscriptionSettings" | SubscriptionSettings | `apps/web/components/settings/SubscriptionSettings.tsx` | status (3) | active, dark, hover | 1 | Settings section for managing the user's subscription. |
| "apps/web/components/settings/UserAvatar::UserAvatar" | UserAvatar | `apps/web/components/settings/UserAvatar.tsx` |  |  | 8 | Displays the user's avatar in settings. |
| "apps/web/components/settings/UserDetails::UserDetails" | UserDetails | `apps/web/components/settings/UserDetails.tsx` |  |  | 1 | Displays the user's account details. |
| "apps/web/components/settings/UserOptions::ThemeSelect" | ThemeSelect | `apps/web/components/settings/UserOptions.tsx` |  |  | 0 | Select control for choosing the UI theme. |
| "apps/web/components/settings/UserOptions::LanguageSelect" | LanguageSelect | `apps/web/components/settings/UserOptions.tsx` |  |  | 0 | Select control for choosing the UI language. |
| "apps/web/components/settings/UserOptions::UserOptions" | UserOptions | `apps/web/components/settings/UserOptions.tsx` |  |  | 1 | Group of user preference controls including theme and language. |
| "apps/web/components/settings/WebhookEventSelector::WebhookEventSelector" | WebhookEventSelector | `apps/web/components/settings/WebhookEventSelector.tsx` |  |  | 2 | Selector for choosing which events a webhook subscribes to. |
| "apps/web/components/settings/WebhookSettings::WebhookPayloadExample" | WebhookPayloadExample | `apps/web/components/settings/WebhookSettings.tsx` |  | disabled, hover, open | 0 | Shows an example webhook payload. |
| "apps/web/components/settings/WebhookSettings::WebhooksEditorDialog" | WebhooksEditorDialog | `apps/web/components/settings/WebhookSettings.tsx` |  | disabled, hover, open | 0 | Dialog for editing webhooks. |
| "apps/web/components/settings/WebhookSettings::EditWebhookDialog" | EditWebhookDialog | `apps/web/components/settings/WebhookSettings.tsx` |  | disabled, hover, open | 0 | Dialog for editing a single webhook. |
| "apps/web/components/settings/WebhookSettings::EditTokenDialog" | EditTokenDialog | `apps/web/components/settings/WebhookSettings.tsx` |  | disabled, hover, open | 0 | Dialog for editing a webhook token. |
| "apps/web/components/settings/WebhookSettings::WebhookRow" | WebhookRow | `apps/web/components/settings/WebhookSettings.tsx` |  | disabled, hover, open | 0 | Row representing one configured webhook. |
| "apps/web/components/settings/WebhookSettings::WebhookSettings" | WebhookSettings | `apps/web/components/settings/WebhookSettings.tsx` |  | disabled, hover, open | 1 | Settings section listing and managing webhooks. |
| "apps/web/components/shared/sidebar/MobileSidebar::MobileSidebar" | MobileSidebar | `apps/web/components/shared/sidebar/MobileSidebar.tsx` |  |  | 1 | Sidebar navigation variant for mobile widths. |
| "apps/web/components/shared/sidebar/ModileSidebarItem::MobileSidebarItem" | MobileSidebarItem | `apps/web/components/shared/sidebar/ModileSidebarItem.tsx` |  | hover | 1 | Navigation item within the mobile sidebar. |
| "apps/web/components/shared/sidebar/Sidebar::Sidebar" | Sidebar | `apps/web/components/shared/sidebar/Sidebar.tsx` |  |  | 1 | Primary shared sidebar navigation. |
| "apps/web/components/shared/sidebar/SidebarItem::SidebarItem" | SidebarItem | `apps/web/components/shared/sidebar/SidebarItem.tsx` |  | hover | 7 | Navigation item within the sidebar. |
| "apps/web/components/shared/sidebar/SidebarLayout::SidebarLayout" | SidebarLayout | `apps/web/components/shared/sidebar/SidebarLayout.tsx` |  |  | 3 | Page layout that places content alongside the sidebar. |
| "apps/web/components/shared/sidebar/SidebarSectionHeading::SidebarSectionHeading" | SidebarSectionHeading | `apps/web/components/shared/sidebar/SidebarSectionHeading.tsx` |  |  | 3 | Heading labeling a group of sidebar items. |
| "apps/web/components/shared/sidebar/SidebarVersion::SidebarVersion" | SidebarVersion | `apps/web/components/shared/sidebar/SidebarVersion.tsx` |  | focus-visible, hover | 2 | Displays version information in the sidebar. |
| "apps/web/components/shared/sidebar/SmartListMarker::SmartListMarker" | SmartListMarker | `apps/web/components/shared/sidebar/SmartListMarker.tsx` |  |  | 1 | Marker indicating a smart list in the sidebar. |
| "apps/web/components/signin/ForgotPasswordForm::ForgotPasswordForm" | ForgotPasswordForm | `apps/web/components/signin/ForgotPasswordForm.tsx` |  |  | 1 | Form for requesting a password reset. |
| "apps/web/components/signin/OAuthAutoRedirect::OAuthAutoRedirect" | OAuthAutoRedirect | `apps/web/components/signin/OAuthAutoRedirect.tsx` |  |  | 1 | Automatically redirects to an OAuth sign-in flow. |
| "apps/web/components/signin/ResetPasswordForm::ResetPasswordForm" | ResetPasswordForm | `apps/web/components/signin/ResetPasswordForm.tsx` |  |  | 1 | Form for setting a new password. |
| "apps/web/components/signin/SignInForm::SignInForm" | SignInForm | `apps/web/components/signin/SignInForm.tsx` |  |  | 1 | Form for signing in to the app. |
| "apps/web/components/signin/SignInProviderButton::SignInProviderButton" | SignInProviderButton | `apps/web/components/signin/SignInProviderButton.tsx` |  |  | 1 | Button used on the sign-in screen to start authentication with a specific identity provider. |
| "apps/web/components/signup/SignUpForm::SignUpForm" | SignUpForm | `apps/web/components/signup/SignUpForm.tsx` |  | hover | 1 | Form for creating a new account on the sign-up page. |
| "apps/web/components/subscription/QuotaProgress::QuotaProgressItem" | QuotaProgressItem | `apps/web/components/subscription/QuotaProgress.tsx` |  |  | 0 | Single row within the quota display showing progress for one subscription quota. |
| "apps/web/components/subscription/QuotaProgress::QuotaProgress" | QuotaProgress | `apps/web/components/subscription/QuotaProgress.tsx` |  |  | 1 | Container that lists the user's subscription quotas and their current usage. |
| "apps/web/components/theme-provider::ThemeProvider" | ThemeProvider | `apps/web/components/theme-provider.tsx` |  |  | 2 | Wrapper that supplies the active theme to the web application tree. |
| "apps/web/components/ui/action-button::ActionButton" | ActionButton | `apps/web/components/ui/action-button.tsx` |  |  | 87 | Button variant intended for triggering an action, built on the base button. |
| "apps/web/components/ui/action-button::ActionButtonWithTooltip" | ActionButtonWithTooltip | `apps/web/components/ui/action-button.tsx` |  |  | 6 | Action button that also displays a tooltip describing the action. |
| "apps/web/components/ui/action-confirming-dialog::ActionConfirmingDialog" | ActionConfirmingDialog | `apps/web/components/ui/action-confirming-dialog.tsx` |  | open | 27 | Dialog that asks the user to confirm before an action is carried out. |
| "apps/web/components/ui/alert::Alert" | Alert | `apps/web/components/ui/alert.tsx` | variant (2) |  | 17 | Container for an inline alert message. |
| "apps/web/components/ui/alert::AlertTitle" | AlertTitle | `apps/web/components/ui/alert.tsx` |  |  | 4 | Heading line inside an alert. |
| "apps/web/components/ui/alert::AlertDescription" | AlertDescription | `apps/web/components/ui/alert.tsx` |  |  | 17 | Body text inside an alert. |
| "apps/web/components/ui/avatar::Avatar" | Avatar | `apps/web/components/ui/avatar.tsx` |  |  | 3 | Root container for a user avatar. |
| "apps/web/components/ui/avatar::AvatarImage" | AvatarImage | `apps/web/components/ui/avatar.tsx` |  |  | 1 | Image element rendered inside an avatar. |
| "apps/web/components/ui/avatar::AvatarFallback" | AvatarFallback | `apps/web/components/ui/avatar.tsx` |  |  | 1 | Placeholder shown in an avatar when the image is unavailable. |
| "apps/web/components/ui/back-button::BackButton" | BackButton | `apps/web/components/ui/back-button.tsx` |  |  | 0 | Button for navigating back to the previous view. |
| "apps/web/components/ui/badge::Badge" | Badge | `apps/web/components/ui/badge.tsx` | variant (4) | dark, focus-visible, hover | 52 | Small label for tagging or status display. |
| "apps/web/components/ui/button::Button" | Button | `apps/web/components/ui/button.tsx` |  | disabled | 204 | Base button primitive for the web app. |
| "apps/web/components/ui/button::ButtonWithTooltip" | ButtonWithTooltip | `apps/web/components/ui/button.tsx` |  | disabled | 23 | Base button paired with a tooltip. |
| "apps/web/components/ui/calendar::Calendar" | Calendar | `apps/web/components/ui/calendar.tsx` |  | aria-disabled, aria-selected, data-[range-end=true], data-[range-middle=true], data-[range-start=true], data-[selected-single=true] | 5 | Date picker calendar grid. |
| "apps/web/components/ui/calendar::CalendarDayButton" | CalendarDayButton | `apps/web/components/ui/calendar.tsx` |  | aria-disabled, aria-selected, data-[range-end=true], data-[range-middle=true], data-[range-start=true], data-[selected-single=true] | 0 | Individual selectable day cell within the calendar. |
| "apps/web/components/ui/card::Card" | Card | `apps/web/components/ui/card.tsx` |  |  | 35 | Surface container for grouping related content. |
| "apps/web/components/ui/card::CardHeader" | CardHeader | `apps/web/components/ui/card.tsx` |  |  | 24 | Top section of a card holding title and description. |
| "apps/web/components/ui/card::CardTitle" | CardTitle | `apps/web/components/ui/card.tsx` |  |  | 22 | Title text within a card header. |
| "apps/web/components/ui/card::CardDescription" | CardDescription | `apps/web/components/ui/card.tsx` |  |  | 20 | Supporting description text within a card header. |
| "apps/web/components/ui/card::CardContent" | CardContent | `apps/web/components/ui/card.tsx` |  |  | 28 | Main body region of a card. |
| "apps/web/components/ui/card::CardFooter" | CardFooter | `apps/web/components/ui/card.tsx` |  |  | 0 | Bottom region of a card, typically for actions. |
| "apps/web/components/ui/collapsible::CollapsibleTriggerTriangle" | CollapsibleTriggerTriangle | `apps/web/components/ui/collapsible.tsx` |  | focus-visible, open | 0 | Collapsible toggle using a triangle indicator. |
| "apps/web/components/ui/collapsible::CollapsibleTriggerChevron" | CollapsibleTriggerChevron | `apps/web/components/ui/collapsible.tsx` |  | focus-visible, open | 2 | Collapsible toggle using a chevron indicator. |
| "apps/web/components/ui/command::Command" | Command | `apps/web/components/ui/command.tsx` |  | data-[disabled=true], data-[selected=true], disabled, placeholder | 13 | Root of the command palette / searchable command menu. |
| "apps/web/components/ui/command::CommandDialog" | CommandDialog | `apps/web/components/ui/command.tsx` |  | data-[disabled=true], data-[selected=true], disabled, placeholder | 0 | Command palette presented inside a dialog. |
| "apps/web/components/ui/command::CommandInput" | CommandInput | `apps/web/components/ui/command.tsx` |  | data-[disabled=true], data-[selected=true], disabled, placeholder | 10 | Search input for filtering command items. |
| "apps/web/components/ui/command::CommandList" | CommandList | `apps/web/components/ui/command.tsx` |  | data-[disabled=true], data-[selected=true], disabled, placeholder | 11 | Scrollable list of command results. |
| "apps/web/components/ui/command::CommandEmpty" | CommandEmpty | `apps/web/components/ui/command.tsx` |  | data-[disabled=true], data-[selected=true], disabled, placeholder | 10 | Empty state shown when no commands match the query. |
| "apps/web/components/ui/command::CommandGroup" | CommandGroup | `apps/web/components/ui/command.tsx` |  | data-[disabled=true], data-[selected=true], disabled, placeholder | 12 | Labeled grouping of related command items. |
| "apps/web/components/ui/command::CommandSeparator" | CommandSeparator | `apps/web/components/ui/command.tsx` |  | data-[disabled=true], data-[selected=true], disabled, placeholder | 1 | Divider between command groups or items. |
| "apps/web/components/ui/command::CommandItem" | CommandItem | `apps/web/components/ui/command.tsx` |  | data-[disabled=true], data-[selected=true], disabled, placeholder | 15 | Single selectable entry in the command list. |
| "apps/web/components/ui/command::CommandShortcut" | CommandShortcut | `apps/web/components/ui/command.tsx` |  | data-[disabled=true], data-[selected=true], disabled, placeholder | 0 | Keyboard shortcut hint displayed alongside a command item. |
| "apps/web/components/ui/copy-button::CopyBtn" | CopyBtn | `apps/web/components/ui/copy-button.tsx` |  |  | 1 | Button that copies associated content to the clipboard. |
| "apps/web/components/ui/copy-button::CopyBtnV2" | CopyBtnV2 | `apps/web/components/ui/copy-button.tsx` |  |  | 2 | Second iteration of the copy-to-clipboard button. |
| "apps/web/components/ui/dialog::DialogOverlay" | DialogOverlay | `apps/web/components/ui/dialog.tsx` | size (2) | data-[state=closed], data-[state=open], disabled, focus-visible, has-[[data-dialog-body]], hover | 2 | Backdrop layer rendered behind an open dialog. |
| "apps/web/components/ui/dialog::DialogContent" | DialogContent | `apps/web/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus-visible, has-[[data-dialog-body]], hover | 36 | The main container of a modal dialog that holds its header, body and footer. |
| "apps/web/components/ui/dialog::DialogHeader" | DialogHeader | `apps/web/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus-visible, has-[[data-dialog-body]], hover | 31 | The top region of a dialog, grouping the title and description. |
| "apps/web/components/ui/dialog::DialogBody" | DialogBody | `apps/web/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus-visible, has-[[data-dialog-body]], hover | 7 | The scrollable or main content area of a dialog between header and footer. |
| "apps/web/components/ui/dialog::DialogFooter" | DialogFooter | `apps/web/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus-visible, has-[[data-dialog-body]], hover | 24 | The bottom region of a dialog, intended for actions such as confirm or cancel buttons. |
| "apps/web/components/ui/dialog::DialogTitle" | DialogTitle | `apps/web/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus-visible, has-[[data-dialog-body]], hover | 35 | The accessible heading text of a dialog. |
| "apps/web/components/ui/dialog::DialogDescription" | DialogDescription | `apps/web/components/ui/dialog.tsx` |  | data-[state=closed], data-[state=open], disabled, focus-visible, has-[[data-dialog-body]], hover | 13 | Supporting descriptive text shown beneath a dialog title. |
| "apps/web/components/ui/dropdown-menu::DropdownMenuSubTrigger" | DropdownMenuSubTrigger | `apps/web/components/ui/dropdown-menu.tsx` | variant (2) | dark, data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top] | 1 | A menu item that opens a nested submenu when hovered or activated. |
| "apps/web/components/ui/dropdown-menu::DropdownMenuSubContent" | DropdownMenuSubContent | `apps/web/components/ui/dropdown-menu.tsx` |  | dark, data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top] | 1 | The panel containing items of a nested submenu. |
| "apps/web/components/ui/dropdown-menu::DropdownMenuContent" | DropdownMenuContent | `apps/web/components/ui/dropdown-menu.tsx` |  | dark, data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top] | 11 | The floating panel that holds a dropdown menu's items. |
| "apps/web/components/ui/dropdown-menu::DropdownMenuItem" | DropdownMenuItem | `apps/web/components/ui/dropdown-menu.tsx` |  | dark, data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top] | 34 | A single selectable action within a dropdown menu. |
| "apps/web/components/ui/dropdown-menu::DropdownMenuCheckboxItem" | DropdownMenuCheckboxItem | `apps/web/components/ui/dropdown-menu.tsx` |  | dark, data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top] | 0 | A dropdown menu item with a toggleable checked state. |
| "apps/web/components/ui/dropdown-menu::DropdownMenuRadioItem" | DropdownMenuRadioItem | `apps/web/components/ui/dropdown-menu.tsx` |  | dark, data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top] | 5 | A dropdown menu item belonging to a mutually exclusive radio group. |
| "apps/web/components/ui/dropdown-menu::DropdownMenuLabel" | DropdownMenuLabel | `apps/web/components/ui/dropdown-menu.tsx` |  | dark, data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top] | 7 | A non-interactive heading used to label a group of menu items. |
| "apps/web/components/ui/dropdown-menu::DropdownMenuSeparator" | DropdownMenuSeparator | `apps/web/components/ui/dropdown-menu.tsx` |  | dark, data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top] | 10 | A visual divider between groups of dropdown menu items. |
| "apps/web/components/ui/dropdown-menu::DropdownMenuShortcut" | DropdownMenuShortcut | `apps/web/components/ui/dropdown-menu.tsx` |  | dark, data-[disabled], data-[side=bottom], data-[side=left], data-[side=right], data-[side=top] | 0 | Secondary text displaying a keyboard shortcut hint alongside a menu item. |
| "apps/web/components/ui/empty::Empty" | Empty | `apps/web/components/ui/empty.tsx` |  |  | 23 | The root container for an empty-state message shown when there is no content to display. |
| "apps/web/components/ui/empty::EmptyHeader" | EmptyHeader | `apps/web/components/ui/empty.tsx` |  |  | 23 | Groups the media, title and description of an empty state. |
| "apps/web/components/ui/empty::EmptyMedia" | EmptyMedia | `apps/web/components/ui/empty.tsx` | variant (2) |  | 19 | Slot for an icon or illustration in an empty state. |
| "apps/web/components/ui/empty::EmptyTitle" | EmptyTitle | `apps/web/components/ui/empty.tsx` |  |  | 23 | The heading text of an empty state. |
| "apps/web/components/ui/empty::EmptyDescription" | EmptyDescription | `apps/web/components/ui/empty.tsx` |  |  | 16 | Explanatory text within an empty state. |
| "apps/web/components/ui/empty::EmptyContent" | EmptyContent | `apps/web/components/ui/empty.tsx` |  |  | 9 | Slot for actions or additional content beneath an empty-state header. |
| "apps/web/components/ui/field::FieldSet" | FieldSet | `apps/web/components/ui/field.tsx` | variant (2) | dark, data-[invalid=true], data-[slot=checkbox-group], data-[variant=label], data-[variant=legend], group-data-[disabled=true]/field | 0 | Groups related form fields together under a shared legend. |
| "apps/web/components/ui/field::FieldLegend" | FieldLegend | `apps/web/components/ui/field.tsx` |  | dark, data-[invalid=true], data-[slot=checkbox-group], data-[variant=label], data-[variant=legend], group-data-[disabled=true]/field | 0 | The caption for a field set. |
| "apps/web/components/ui/field::FieldGroup" | FieldGroup | `apps/web/components/ui/field.tsx` |  | dark, data-[invalid=true], data-[slot=checkbox-group], data-[variant=label], data-[variant=legend], group-data-[disabled=true]/field | 0 | A layout wrapper that stacks multiple fields with consistent spacing. |
| "apps/web/components/ui/field::Field" | Field | `apps/web/components/ui/field.tsx` | orientation (3) | dark, data-[invalid=true], data-[slot=checkbox-group], data-[variant=label], data-[variant=legend], group-data-[disabled=true]/field | 1 | The wrapper for a single form field, combining its label, control, description and error. |
| "apps/web/components/ui/field::FieldContent" | FieldContent | `apps/web/components/ui/field.tsx` |  | dark, data-[invalid=true], data-[slot=checkbox-group], data-[variant=label], data-[variant=legend], group-data-[disabled=true]/field | 1 | Wraps the control and its supporting text inside a field. |
| "apps/web/components/ui/field::FieldLabel" | FieldLabel | `apps/web/components/ui/field.tsx` |  | dark, data-[invalid=true], data-[slot=checkbox-group], data-[variant=label], data-[variant=legend], group-data-[disabled=true]/field | 4 | The label associated with a field's input control. |
| "apps/web/components/ui/field::FieldTitle" | FieldTitle | `apps/web/components/ui/field.tsx` |  | dark, data-[invalid=true], data-[slot=checkbox-group], data-[variant=label], data-[variant=legend], group-data-[disabled=true]/field | 1 | A title text element for a field, used where a label element is not appropriate. |
| "apps/web/components/ui/field::FieldDescription" | FieldDescription | `apps/web/components/ui/field.tsx` |  | dark, data-[invalid=true], data-[slot=checkbox-group], data-[variant=label], data-[variant=legend], group-data-[disabled=true]/field | 0 | Helper text explaining a field's purpose or expected input. |
| "apps/web/components/ui/field::FieldSeparator" | FieldSeparator | `apps/web/components/ui/field.tsx` |  | dark, data-[invalid=true], data-[slot=checkbox-group], data-[variant=label], data-[variant=legend], group-data-[disabled=true]/field | 0 | A divider placed between fields or field groups. |
| "apps/web/components/ui/field::FieldError" | FieldError | `apps/web/components/ui/field.tsx` |  | dark, data-[invalid=true], data-[slot=checkbox-group], data-[variant=label], data-[variant=legend], group-data-[disabled=true]/field | 1 | Displays validation error text for a field. |
| "apps/web/components/ui/file-picker-button::FilePickerButton" | FilePickerButton | `apps/web/components/ui/file-picker-button.tsx` |  |  | 3 | A button that opens the native file chooser so a user can select files. |
| "apps/web/components/ui/form::FormField" | FormField | `apps/web/components/ui/form.tsx` |  |  | 0 | Connects a form control to form state for a named field. |
| "apps/web/components/ui/form::FormItem" | FormItem | `apps/web/components/ui/form.tsx` |  |  | 79 | The wrapper for one form field's label, control, description and message. |
| "apps/web/components/ui/form::FormLabel" | FormLabel | `apps/web/components/ui/form.tsx` |  |  | 66 | The label for a form field, tied to its control. |
| "apps/web/components/ui/form::FormControl" | FormControl | `apps/web/components/ui/form.tsx` |  |  | 79 | Wraps the input element and wires up accessibility attributes for the field. |
| "apps/web/components/ui/form::FormDescription" | FormDescription | `apps/web/components/ui/form.tsx` |  |  | 10 | Helper text describing a form field. |
| "apps/web/components/ui/form::FormMessage" | FormMessage | `apps/web/components/ui/form.tsx` |  |  | 71 | Displays a form field's validation message. |
| "apps/web/components/ui/formatted-date::FormattedDate" | FormattedDate | `apps/web/components/ui/formatted-date.tsx` |  |  | 5 | Renders a date value in a formatted, human-readable form. |
| "apps/web/components/ui/full-page-spinner::FullPageSpinner" | FullPageSpinner | `apps/web/components/ui/full-page-spinner.tsx` |  |  | 21 | A loading indicator that covers the full page while content is being loaded. |
| "apps/web/components/ui/info-tooltip::InfoTooltip" | InfoTooltip | `apps/web/components/ui/info-tooltip.tsx` | variant (2) |  | 4 | Small informational affordance that reveals explanatory text on hover or focus, used to clarify a label or field without adding permanent copy. |
| "apps/web/components/ui/input::Input" | Input | `apps/web/components/ui/input.tsx` | variant (2) | aria-[invalid=true], dark, disabled, file, focus-visible, hover | 80 | Base single-line text field for forms; the foundation other inputs build on. |
| "apps/web/components/ui/kbd::Kbd" | Kbd | `apps/web/components/ui/kbd.tsx` |  | dark | 2 | Renders a single keyboard key as an inline, key-cap styled element for documenting shortcuts. |
| "apps/web/components/ui/kbd::KbdGroup" | KbdGroup | `apps/web/components/ui/kbd.tsx` |  | dark | 0 | Groups several @apps/web/components/ui/kbd::Kbd elements to present a key combination or sequence. |
| "apps/web/components/ui/label::Label" | Label | `apps/web/components/ui/label.tsx` |  | peer-disabled | 38 | Accessible caption associated with a form control such as @apps/web/components/ui/input::Input or @apps/web/components/ui/switch::Switch. |
| "apps/web/components/ui/markdown/markdown-editor::MarkdownEditor" | MarkdownEditor | `apps/web/components/ui/markdown/markdown-editor.tsx` |  | dark, focus-visible | 2 | Rich editing surface for authoring markdown content, paired with @apps/web/components/ui/markdown/plugins/toolbar-plugin::ToolbarPlugin for formatting actions. |
| "apps/web/components/ui/markdown/markdown-readonly::PreWithCopyBtn" | PreWithCopyBtn | `apps/web/components/ui/markdown/markdown-readonly.tsx` |  | dark, group-hover | 0 | Preformatted code block wrapper that adds a copy-to-clipboard button, used inside rendered markdown. |
| "apps/web/components/ui/markdown/markdown-readonly::MarkdownReadonly" | MarkdownReadonly | `apps/web/components/ui/markdown/markdown-readonly.tsx` |  | dark, group-hover | 3 | Renders stored markdown as read-only formatted content, using @apps/web/components/ui/markdown/markdown-readonly::PreWithCopyBtn for code. |
| "apps/web/components/ui/markdown/plugins/toolbar-plugin::MarkdownToolTip" | MarkdownToolTip | `apps/web/components/ui/markdown/plugins/toolbar-plugin.tsx` |  | hover | 0 | Tooltip variant specific to the markdown toolbar, describing what each formatting button does. |
| "apps/web/components/ui/markdown/plugins/toolbar-plugin::ToolbarPlugin" | ToolbarPlugin | `apps/web/components/ui/markdown/plugins/toolbar-plugin.tsx` |  | hover | 1 | Formatting toolbar for @apps/web/components/ui/markdown/markdown-editor::MarkdownEditor, exposing editor commands as buttons. |
| "apps/web/components/ui/multiple-choice-dialog::MultipleChoiceDialog" | MultipleChoiceDialog | `apps/web/components/ui/multiple-choice-dialog.tsx` |  | open | 1 | Modal dialog that asks the user to pick one option from a set of choices before continuing. |
| "apps/web/components/ui/page-header::PageHeader" | PageHeader | `apps/web/components/ui/page-header.tsx` |  |  | 6 | Top-of-page heading area that establishes the page title and context. |
| "apps/web/components/ui/password-input::PasswordInput" | PasswordInput | `apps/web/components/ui/password-input.tsx` |  | after, dark, focus-visible, hover | 12 | Specialization of @apps/web/components/ui/input::Input for secret entry, with masked characters. |
| "apps/web/components/ui/progress::Progress" | Progress | `apps/web/components/ui/progress.tsx` |  |  | 4 | Horizontal bar communicating determinate completion of a task or quantity. |
| "apps/web/components/ui/radio-group::RadioGroup" | RadioGroup | `apps/web/components/ui/radio-group.tsx` |  | disabled, focus-visible | 3 | Container managing a mutually exclusive set of @apps/web/components/ui/radio-group::RadioGroupItem options. |
| "apps/web/components/ui/radio-group::RadioGroupItem" | RadioGroupItem | `apps/web/components/ui/radio-group.tsx` |  | disabled, focus-visible | 5 | Single selectable option within a @apps/web/components/ui/radio-group::RadioGroup. |
| "apps/web/components/ui/relative-time::RelativeTime" | RelativeTime | `apps/web/components/ui/relative-time.tsx` |  |  | 2 | Displays a timestamp as a human-readable relative phrase rather than an absolute date. |
| "apps/web/components/ui/scroll-area::ScrollArea" | ScrollArea | `apps/web/components/ui/scroll-area.tsx` |  |  | 1 | Styled scrolling container that constrains overflowing content and hosts @apps/web/components/ui/scroll-area::ScrollBar. |
| "apps/web/components/ui/scroll-area::ScrollBar" | ScrollBar | `apps/web/components/ui/scroll-area.tsx` |  |  | 0 | Custom scrollbar track and thumb rendered inside @apps/web/components/ui/scroll-area::ScrollArea. |
| "apps/web/components/ui/select::SelectTrigger" | SelectTrigger | `apps/web/components/ui/select.tsx` |  | aria-[invalid=true], dark, data-[disabled], data-[placeholder], data-[side=bottom], data-[side=left] | 29 | Button-like control that displays the current value and opens @apps/web/components/ui/select::SelectContent. |
| "apps/web/components/ui/select::SelectScrollUpButton" | SelectScrollUpButton | `apps/web/components/ui/select.tsx` |  | aria-[invalid=true], dark, data-[disabled], data-[placeholder], data-[side=bottom], data-[side=left] | 1 | Affordance at the top of a long option list that scrolls it upward. |
| "apps/web/components/ui/select::SelectScrollDownButton" | SelectScrollDownButton | `apps/web/components/ui/select.tsx` |  | aria-[invalid=true], dark, data-[disabled], data-[placeholder], data-[side=bottom], data-[side=left] | 1 | Affordance at the bottom of a long option list that scrolls it downward. |
| "apps/web/components/ui/select::SelectContent" | SelectContent | `apps/web/components/ui/select.tsx` |  | aria-[invalid=true], dark, data-[disabled], data-[placeholder], data-[side=bottom], data-[side=left] | 29 | Popover panel containing the dropdown's option list, labels and separators. |
| "apps/web/components/ui/select::SelectLabel" | SelectLabel | `apps/web/components/ui/select.tsx` |  | aria-[invalid=true], dark, data-[disabled], data-[placeholder], data-[side=bottom], data-[side=left] | 0 | Non-interactive heading used to title a group of options within @apps/web/components/ui/select::SelectContent. |
| "apps/web/components/ui/select::SelectItem" | SelectItem | `apps/web/components/ui/select.tsx` |  | aria-[invalid=true], dark, data-[disabled], data-[placeholder], data-[side=bottom], data-[side=left] | 82 | Individual selectable option within a select dropdown. |
| "apps/web/components/ui/select::SelectSeparator" | SelectSeparator | `apps/web/components/ui/select.tsx` |  | aria-[invalid=true], dark, data-[disabled], data-[placeholder], data-[side=bottom], data-[side=left] | 0 | Thin divider between option groups inside @apps/web/components/ui/select::SelectContent. |
| "apps/web/components/ui/separator::Separator" | Separator | `apps/web/components/ui/separator.tsx` |  |  | 18 | General-purpose horizontal or vertical rule for visually dividing content. |
| "apps/web/components/ui/skeleton::Skeleton" | Skeleton | `apps/web/components/ui/skeleton.tsx` |  |  | 70 | Placeholder block that stands in for content while it loads. |
| "apps/web/components/ui/slider::Slider" | Slider | `apps/web/components/ui/slider.tsx` |  | disabled, focus-visible | 5 | Draggable track control for choosing a numeric value within a continuous range. |
| "apps/web/components/ui/slider::StepperSlider" | StepperSlider | `apps/web/components/ui/slider.tsx` |  | disabled, focus-visible | 2 | Variant of @apps/web/components/ui/slider::Slider that snaps to discrete steps. |
| "apps/web/components/ui/sonner::Toaster" | Toaster | `apps/web/components/ui/sonner.tsx` | variant (2) | dark, group-[.toast], group-[.toaster] | 2 | Mount point for transient toast notifications shown in response to user actions. |
| "apps/web/components/ui/spinner::LoadingSpinner" | LoadingSpinner | `apps/web/components/ui/spinner.tsx` |  |  | 19 | Indeterminate loading indicator for in-progress operations. |
| "apps/web/components/ui/stat-tile::StatTile" | StatTile | `apps/web/components/ui/stat-tile.tsx` |  | focus-visible, hover | 10 | Compact card presenting a single headline metric for dashboards or summaries. |
| "apps/web/components/ui/switch::Switch" | Switch | `apps/web/components/ui/switch.tsx` |  | after, dark, data-[state=checked], data-[state=unchecked], disabled, focus-visible | 26 | Binary on/off toggle for boolean settings. |
| "apps/web/components/ui/table::Table" | Table | `apps/web/components/ui/table.tsx` |  | data-[state=selected], first, hover, last | 13 | Root element for tabular data; composes header, body, footer and row parts. |
| "apps/web/components/ui/table::TableHeader" | TableHeader | `apps/web/components/ui/table.tsx` |  | data-[state=selected], first, hover, last | 11 | Header section of @apps/web/components/ui/table::Table containing column heading rows. |
| "apps/web/components/ui/table::TableBody" | TableBody | `apps/web/components/ui/table.tsx` |  | data-[state=selected], first, hover, last | 13 | Body section holding the data rows of @apps/web/components/ui/table::Table. |
| "apps/web/components/ui/table::TableFooter" | TableFooter | `apps/web/components/ui/table.tsx` |  | data-[state=selected], first, hover, last | 0 | Footer section of @apps/web/components/ui/table::Table for totals or summary rows. |
| "apps/web/components/ui/table::TableRow" | TableRow | `apps/web/components/ui/table.tsx` |  | data-[state=selected], first, hover, last | 40 | Single row within a table section. |
| "apps/web/components/ui/table::TableHead" | TableHead | `apps/web/components/ui/table.tsx` |  | data-[state=selected], first, hover, last | 44 | Column heading cell used inside @apps/web/components/ui/table::TableHeader. |
| "apps/web/components/ui/table::TableCell" | TableCell | `apps/web/components/ui/table.tsx` |  | data-[state=selected], first, hover, last | 75 | Body cell primitive for the web app's data table. |
| "apps/web/components/ui/table::TableCaption" | TableCaption | `apps/web/components/ui/table.tsx` |  | data-[state=selected], first, hover, last | 0 | Caption text attached to a table, describing its contents. |
| "apps/web/components/ui/table::StackedLabel" | StackedLabel | `apps/web/components/ui/table.tsx` |  | data-[state=selected], first, hover, last | 7 | Table helper that stacks a label alongside its value, part of the table module. |
| "apps/web/components/ui/tabs::TabsList" | TabsList | `apps/web/components/ui/tabs.tsx` |  | data-[state=active], disabled, focus-visible | 2 | Container that lays out the set of tab triggers. |
| "apps/web/components/ui/tabs::TabsTrigger" | TabsTrigger | `apps/web/components/ui/tabs.tsx` |  | data-[state=active], disabled, focus-visible | 7 | Individual clickable tab that selects its associated content panel. |
| "apps/web/components/ui/tabs::TabsContent" | TabsContent | `apps/web/components/ui/tabs.tsx` |  | data-[state=active], disabled, focus-visible | 2 | Panel shown when its matching tab trigger is active. |
| "apps/web/components/ui/textarea::Textarea" | Textarea | `apps/web/components/ui/textarea.tsx` |  | placeholder | 12 | Multi-line text input for the web app's forms. |
| "apps/web/components/ui/toast::ToastViewport" | ToastViewport | `apps/web/components/ui/toast.tsx` |  | data-[state=closed], data-[state=open], data-[swipe=cancel], data-[swipe=end], data-[swipe=move], disabled | 0 | Fixed region where toasts are rendered and stacked. |
| "apps/web/components/ui/toast::Toast" | Toast | `apps/web/components/ui/toast.tsx` | variant (2) | data-[state=closed], data-[state=open], data-[swipe=cancel], data-[swipe=end], data-[swipe=move], disabled | 0 | A single transient notification message. |
| "apps/web/components/ui/toast::ToastAction" | ToastAction | `apps/web/components/ui/toast.tsx` |  | data-[state=closed], data-[state=open], data-[swipe=cancel], data-[swipe=end], data-[swipe=move], disabled | 0 | Optional action button inside a toast. |
| "apps/web/components/ui/toast::ToastClose" | ToastClose | `apps/web/components/ui/toast.tsx` |  | data-[state=closed], data-[state=open], data-[swipe=cancel], data-[swipe=end], data-[swipe=move], disabled | 0 | Dismiss control for a toast. |
| "apps/web/components/ui/toast::ToastTitle" | ToastTitle | `apps/web/components/ui/toast.tsx` |  | data-[state=closed], data-[state=open], data-[swipe=cancel], data-[swipe=end], data-[swipe=move], disabled | 0 | Heading text of a toast. |
| "apps/web/components/ui/toast::ToastDescription" | ToastDescription | `apps/web/components/ui/toast.tsx` |  | data-[state=closed], data-[state=open], data-[swipe=cancel], data-[swipe=end], data-[swipe=move], disabled | 0 | Supporting body text of a toast. |
| "apps/web/components/ui/toggle::Toggle" | Toggle | `apps/web/components/ui/toggle.tsx` | variant (2), size (3) | data-[state=on], disabled, focus-visible, hover | 3 | Two-state pressable control for switching an option on or off. |
| "apps/web/components/ui/tooltip::TooltipTrigger" | TooltipTrigger | `apps/web/components/ui/tooltip.tsx` |  | data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed] | 33 | Element that opens a tooltip on hover or focus. |
| "apps/web/components/ui/tooltip::TooltipContent" | TooltipContent | `apps/web/components/ui/tooltip.tsx` |  | data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed] | 33 | Floating label content shown by a tooltip. |
| "apps/web/components/ui/user-avatar::UserAvatar" | UserAvatar | `apps/web/components/ui/user-avatar.tsx` |  |  | 8 | Displays the current user's avatar image or fallback. |
| "apps/web/components/utils/BookmarkSavedToast::BookmarkSavedToast" | BookmarkSavedToast | `apps/web/components/utils/BookmarkSavedToast.tsx` |  | hover | 2 | Toast confirming that a bookmark has been saved. |
| "apps/web/components/utils/ValidAccountCheck::ValidAccountCheck" | ValidAccountCheck | `apps/web/components/utils/ValidAccountCheck.tsx` |  |  | 1 | Utility wrapper that verifies the account is valid before rendering. |
| "apps/web/components/wrapped/ShareButton::ShareButton" | ShareButton | `apps/web/components/wrapped/ShareButton.tsx` |  | dark, hover | 1 | Button for sharing the wrapped summary. |
| "apps/web/components/wrapped/WrappedContent::WrappedContent" | WrappedContent | `apps/web/components/wrapped/WrappedContent.tsx` |  |  | 1 | Main content of the wrapped summary view. |
| "apps/web/components/wrapped/WrappedModal::WrappedModal" | WrappedModal | `apps/web/components/wrapped/WrappedModal.tsx` |  | hover, open | 0 | Modal dialog that presents the wrapped summary. |
| "apps/web/lib/i18n/provider::CustomI18nextProvider" | CustomI18nextProvider | `apps/web/lib/i18n/provider.tsx` |  |  | 1 | Context provider supplying i18next translations to the web app. |
| "apps/web/lib/providers::Providers" | Providers | `apps/web/lib/providers.tsx` |  |  | 4 | Composes the web app's top-level context providers. |
| "apps/web/lib/readerSettings::ReaderSettingsProvider" | ReaderSettingsProvider | `apps/web/lib/readerSettings.tsx` |  |  | 4 | Context provider for reader view settings. |
| "apps/web/lib/userSettings::UserSettingsContextProvider" | UserSettingsContextProvider | `apps/web/lib/userSettings.tsx` |  |  | 3 | Context provider for user-level settings. |
| "docs/src/theme/DocSidebarItem/Category/index::CollapseButton" | CollapseButton | `docs/src/theme/DocSidebarItem/Category/index.tsx` |  |  | 0 | Button that expands or collapses a docs sidebar category. |
| "docs/src/theme/DocSidebarItem/Category/index::DocSidebarItemCategory" | DocSidebarItemCategory | `docs/src/theme/DocSidebarItem/Category/index.tsx` |  |  | 0 | Swizzled Docusaurus sidebar category item for the docs site. |
| "packages/benchmarks/setup/html/hello.html::PackagesBenchmarksSetupHtmlHelloPage" | PackagesBenchmarksSetupHtmlHelloPage | `packages/benchmarks/setup/html/hello.html` |  |  | 0 | Static HTML fixture page used by the benchmarks setup. |
| "packages/e2e_tests/setup/html/article.html::PackagesE2eTestsSetupHtmlArticlePage" | PackagesE2eTestsSetupHtmlArticlePage | `packages/e2e_tests/setup/html/article.html` |  |  | 0 | Static article HTML fixture used by end-to-end tests. |
| "packages/e2e_tests/setup/html/hello.html::PackagesE2eTestsSetupHtmlHelloPage" | PackagesE2eTestsSetupHtmlHelloPage | `packages/e2e_tests/setup/html/hello.html` |  |  | 0 | Static hello HTML fixture used by end-to-end tests. |
| "packages/shared-react/components/BookmarkHtmlHighlighter::HighlightForm" | HighlightForm | `packages/shared-react/components/BookmarkHtmlHighlighter.tsx` |  | dark, focus-visible, hover, open | 0 | Form for creating or editing a highlight on bookmarked HTML. |
| "packages/shared-react/components/BookmarkHtmlHighlighter::HighlightDock" | HighlightDock | `packages/shared-react/components/BookmarkHtmlHighlighter.tsx` |  |  | 0 | Docked toolbar for highlight actions within the highlighter. |
| "packages/shared-react/components/BookmarkHtmlHighlighter::BookmarkHTMLHighlighter" | BookmarkHTMLHighlighter | `packages/shared-react/components/BookmarkHtmlHighlighter.tsx` |  | dark, focus-visible, hover, open | 2 | Renders bookmarked HTML content with text highlighting support, shared across apps. |
| "packages/shared-react/components/ScrollProgressTracker::ScrollProgressTracker" | ScrollProgressTracker | `packages/shared-react/components/ScrollProgressTracker.tsx` |  |  | 2 | Tracks scroll progress through content, shared across apps. |
| "packages/shared-react/components/ui/button::Button" | Button | `packages/shared-react/components/ui/button.tsx` | variant (10), size (7) | aria-[invalid=true], dark, disabled, focus-visible, has-[>svg], hover | 205 | Shared button primitive used across web and mobile surfaces. |
| "packages/shared-react/components/ui/popover::PopoverContent" | PopoverContent | `packages/shared-react/components/ui/popover.tsx` |  | data-[side=bottom], data-[side=left], data-[side=right], data-[side=top], data-[state=closed], data-[state=open] | 17 | Shared floating popover content container. |
| "packages/shared-react/components/ui/textarea::Textarea" | Textarea | `packages/shared-react/components/ui/textarea.tsx` |  | aria-[invalid=true], dark, disabled, focus-visible, placeholder, selection | 12 | Shared multi-line text input primitive. |
| "packages/shared-react/hooks/bookmark-grid-context::BookmarkGridContextProvider" | BookmarkGridContextProvider | `packages/shared-react/hooks/bookmark-grid-context.tsx` |  |  | 1 | Context provider for bookmark grid layout state. |
| "packages/shared-react/hooks/bookmark-list-context::BookmarkListContextProvider" | BookmarkListContextProvider | `packages/shared-react/hooks/bookmark-list-context.tsx` |  |  | 1 | Context provider for bookmark list state. |
| "packages/shared-react/hooks/reader-settings::ReaderSettingsProvider" | ReaderSettingsProvider | `packages/shared-react/hooks/reader-settings.tsx` |  |  | 4 | Context provider from the shared-react hooks folder that supplies reader settings to its descendants. The list does not state which settings it holds. |
| "packages/shared-react/providers/client-config-provider::ClientConfigProvider" | ClientConfigProvider | `packages/shared-react/providers/client-config-provider.tsx` |  |  | 2 | Context provider that exposes client configuration to the component tree. No further detail is given. |
| "packages/shared-react/providers/trpc-provider::TRPCSettingsProvider" | TRPCSettingsProvider | `packages/shared-react/providers/trpc-provider.tsx` |  |  | 2 | Context provider that supplies tRPC-related settings to the app. No further detail is given. |

### Variants, in full

#### Text (`apps/mobile/components/ui/Text.tsx`:37)

Always applied: `text-foreground`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `largeTitle` | `text-4xl` | 1 |
| `variant` | `title1` | `text-2xl` | 3 |
| `variant` | `title2` | `text-[22px] leading-7` | 0 |
| `variant` | `title3` | `text-xl` | 2 |
| `variant` | `heading` | `text-[17px] font-semibold leading-6` | 4 |
| `variant` | `body` _(default)_ | `text-[17px] leading-6` | 3 |
| `variant` | `callout` | `text-base` | 0 |
| `variant` | `subhead` | `text-[15px] leading-5` | 12 |
| `variant` | `footnote` | `text-[13px] leading-5` | 65 |
| `variant` | `caption1` | `text-xs leading-4` | 8 |
| `variant` | `caption2` | `text-[11px] leading-4` | 1 |
| `color` | `primary` _(default)_ | _none_ | 0 |
| `color` | `secondary` | `text-muted-foreground` | 0 |
| `color` | `tertiary` | `text-muted-foreground` | 67 |
| `color` | `quarternary` | "text-muted-foreground/70" | 0 |

Rendered 239 time(s) in 58 other file(s).

#### Button (`apps/browser-extension/src/components/ui/button.tsx`:45)

Always applied: `inline-flex items-center justify-center whitespace-nowrap rounded-md text-sm font-medium ring-offset-background transition-all focus-visible:outline-none focus-visible:ring-[3px] focus-visible:ring-ring/50 disabled:pointer-events-none disabled:opacity-50`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `default` _(default)_ | `bg-primary text-primary-foreground hover:bg-primary/90` | 2 |
| `variant` | `destructive` | `bg-destructive text-destructive-foreground hover:bg-destructive/90 dark:bg-destructive/60` | 5 |
| `variant` | `outline` | `border border-input bg-background shadow-sm hover:bg-accent hover:text-accent-foreground dark:bg-input/30 dark:hover:bg-input/50` | 66 |
| `variant` | `secondary` | `bg-secondary text-secondary-foreground hover:bg-secondary/80` | 16 |
| `variant` | `ghost` | `hover:bg-accent hover:text-accent-foreground` | 59 |
| `variant` | `link` | `text-primary underline-offset-4 hover:underline` | 1 |
| `size` | `default` _(default)_ | `h-10 px-4 py-2` | 0 |
| `size` | `sm` | `h-9 rounded-md px-3` | 51 |
| `size` | `lg` | `h-11 rounded-md px-8` | 4 |
| `size` | `icon` | `h-10 w-10` | 18 |

States targeted in this file: `dark`, `disabled`, `focus-visible`, `hover`

Rendered 205 time(s) in 109 other file(s).

#### Button (`apps/landing/components/ui/button.tsx`:45)

Always applied: `inline-flex items-center justify-center whitespace-nowrap rounded-lg text-base font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `default` _(default)_ | `bg-primary text-primary-foreground hover:bg-primary/90` | 2 |
| `variant` | `brand` | `bg-[#171717] text-[#f8fafc] hover:bg-[#171717]/90` | 0 |
| `variant` | `destructive` | `bg-destructive text-destructive-foreground hover:bg-destructive/90` | 5 |
| `variant` | `outline` | `border border-input bg-background hover:bg-accent hover:text-accent-foreground` | 66 |
| `variant` | `secondary` | `bg-secondary text-secondary-foreground hover:bg-secondary/80` | 16 |
| `variant` | `ghost` | `hover:bg-accent hover:text-accent-foreground` | 59 |
| `variant` | `link` | `text-primary underline-offset-4 hover:underline` | 1 |
| `size` | `default` _(default)_ | `h-10 px-4 py-2` | 0 |
| `size` | `sm` | `h-9 rounded-lg px-3` | 51 |
| `size` | `lg` | `h-12 rounded-lg px-8` | 4 |
| `size` | `icon` | `size-10` | 18 |

States targeted in this file: `disabled`, `focus-visible`, `hover`

Rendered 205 time(s) in 109 other file(s).

#### Button (`apps/mobile/components/ui/Button.tsx`:154)

Always applied: `flex-row items-center justify-center gap-2`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `primary` _(default)_ | `ios:active:opacity-80 bg-primary` | 2 |
| `variant` | `secondary` | `ios:border-primary ios:active:bg-primary/5 border border-foreground/40` | 16 |
| `variant` | `tonal` | `ios:bg-primary/10 dark:ios:bg-primary/10 ios:active:bg-primary/15 bg-primary/15 dark:bg-primary/30` | 1 |
| `variant` | `plain` | `ios:active:opacity-70` | 4 |
| `variant` | `destructive` | `ios:bg-destructive border border-destructive/5 bg-destructive/80` | 5 |
| `size` | `none` | _none_ | 28 |
| `size` | `sm` | `rounded-full px-2.5 py-1` | 51 |
| `size` | `md` _(default)_ | `ios:rounded-lg ios:py-1.5 ios:px-3.5 rounded-full px-5 py-2` | 0 |
| `size` | `lg` | `ios:py-2 gap-2 rounded-xl px-5 py-2.5` | 4 |
| `size` | `icon` | `ios:rounded-lg h-10 w-10 rounded-full` | 18 |

States targeted in this file: `active`, `dark`

Rendered 205 time(s) in 109 other file(s).

#### Button (`packages/shared-react/components/ui/button.tsx`:54)

Always applied: `inline-flex items-center justify-center gap-2 whitespace-nowrap rounded-md text-sm font-medium transition-all focus-visible:outline-none focus-visible:ring-[3px] focus-visible:ring-ring/50 disabled:pointer-events-none disabled:opacity-50 aria-[invalid=true]:border-destructive aria-[invalid=true]:ring-destructive/20 dark:aria-[invalid=true]:ring-destructive/40 [&_svg:not([class*='size-'])]:size-4 [&_svg]:pointer-events-none [&_svg]:shrink-0`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `none` | _none_ | 2 |
| `variant` | `default` _(default)_ | `bg-primary text-primary-foreground hover:bg-primary/90` | 2 |
| `variant` | `destructive` | `bg-destructive text-destructive-foreground hover:bg-destructive/90 focus-visible:ring-destructive/20 dark:bg-red-600 dark:text-white dark:hover:bg-red-700 dark:focus-visible:ring-destructive/40` | 5 |
| `variant` | `destructiveOutline` | `border border-destructive bg-transparent text-destructive hover:bg-destructive/90 hover:text-destructive-foreground dark:hover:bg-red-600 dark:hover:text-white` | 0 |
| `variant` | `outline` | `border border-border bg-background shadow-sm hover:bg-accent hover:text-accent-foreground dark:bg-accent/60 dark:hover:bg-accent` | 66 |
| `variant` | `secondary` | `bg-secondary text-secondary-foreground hover:bg-secondary/80` | 16 |
| `variant` | `ghost` | `hover:bg-accent hover:text-accent-foreground focus-visible:ring-0 dark:hover:bg-accent/50` | 59 |
| `variant` | `ghostDestructive` | `text-destructive hover:bg-destructive/10 hover:text-destructive focus-visible:ring-0 dark:hover:bg-destructive/20` | 4 |
| `variant` | `border` | `border border-input hover:bg-accent` | 0 |
| `variant` | `link` | `text-primary underline-offset-4 hover:underline` | 1 |
| `size` | `none` | _none_ | 28 |
| `size` | `default` _(default)_ | `h-10 px-4 py-2 has-[>svg]:px-3` | 0 |
| `size` | `sm` | `h-9 gap-1.5 rounded-md px-3 has-[>svg]:px-2.5` | 51 |
| `size` | `lg` | `h-11 rounded-md px-8 has-[>svg]:px-6` | 4 |
| `size` | `icon` | `size-10` | 18 |
| `size` | `icon-sm` | `size-8` | 3 |
| `size` | `icon-xs` | `size-6` | 0 |

States targeted in this file: `aria-[invalid=true]`, `dark`, `disabled`, `focus-visible`, `has-[>svg]`, `hover`

Rendered 205 time(s) in 109 other file(s).

#### Input (`apps/web/components/ui/input.tsx`:16)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `default` | _declared by the prop type only_ | 0 |
| `variant` | `filled` | _declared by the prop type only_ | 3 |

States targeted in this file: `aria-[invalid=true]`, `dark`, `disabled`, `file`, `focus-visible`, `hover`, `placeholder`, `selection`

2 conditional class branch(es) in this file are not a named variant.

Rendered 80 time(s) in 46 other file(s).

#### Badge (`apps/browser-extension/src/components/ui/badge.tsx`:33)

Always applied: `inline-flex items-center rounded-full border px-2.5 py-0.5 text-xs font-semibold transition-colors focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `default` _(default)_ | `border-transparent bg-primary text-primary-foreground hover:bg-primary/80` | 0 |
| `variant` | `secondary` | `border-transparent bg-secondary text-secondary-foreground hover:bg-secondary/80` | 29 |
| `variant` | `destructive` | `border-transparent bg-destructive text-destructive-foreground hover:bg-destructive/80` | 3 |
| `variant` | `outline` | `text-foreground` | 11 |

States targeted in this file: `focus`, `hover`

Rendered 52 time(s) in 16 other file(s).

#### Badge (`apps/web/components/ui/badge.tsx`:32)

Always applied: `inline-flex items-center rounded-full border px-2.5 py-0.5 text-xs font-semibold transition-colors focus-visible:border-ring focus-visible:outline-none focus-visible:ring-[3px] focus-visible:ring-ring/50`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `default` _(default)_ | `border-transparent bg-primary text-primary-foreground hover:bg-primary/80` | 0 |
| `variant` | `secondary` | `border-transparent bg-secondary text-secondary-foreground hover:bg-secondary/80` | 29 |
| `variant` | `destructive` | `border-transparent bg-destructive text-destructive-foreground hover:bg-destructive/80 dark:bg-destructive/60` | 3 |
| `variant` | `outline` | `text-foreground` | 11 |

States targeted in this file: `dark`, `focus-visible`, `hover`

Rendered 52 time(s) in 16 other file(s).

#### IconTooltip (`apps/web/components/dashboard/preview/IconControl.tsx`:17)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `side` | `top` | _declared by the prop type only_ | 0 |
| `side` | `bottom` | _declared by the prop type only_ | 14 |
| `side` | `left` | _declared by the prop type only_ | 0 |
| `side` | `right` | _declared by the prop type only_ | 0 |

States targeted in this file: `hover`

Rendered 29 time(s) in 11 other file(s).

#### EmptyMedia (`apps/web/components/ui/empty.tsx`:49)

Always applied: `mb-2 flex shrink-0 items-center justify-center [&_svg]:pointer-events-none [&_svg]:shrink-0`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `default` _(default)_ | `bg-transparent` | 0 |
| `variant` | `icon` | `flex size-10 shrink-0 items-center justify-center rounded-lg bg-muted text-foreground [&_svg:not([class*='size-'])]:size-6` | 19 |

Rendered 19 time(s) in 17 other file(s).

#### Alert (`apps/web/components/ui/alert.tsx`:23)

Always applied: `relative w-full rounded-lg border p-4 [&>svg+div]:translate-y-[-3px] [&>svg]:absolute [&>svg]:left-4 [&>svg]:top-4 [&>svg]:text-foreground [&>svg~*]:pl-7`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `default` _(default)_ | `bg-background text-foreground` | 0 |
| `variant` | `destructive` | `border-destructive/50 text-destructive [&>svg]:text-destructive` | 11 |

Rendered 17 time(s) in 13 other file(s).

#### SettingsScreen (`apps/mobile/components/settings/settings-list.tsx`:20)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `tone` | `default` | _declared by the prop type only_ | 0 |
| `tone` | `destructive` | _declared by the prop type only_ | 0 |
| `tone` | `primary` | _declared by the prop type only_ | 0 |

States targeted in this file: `active`, `checked`

2 conditional class branch(es) in this file are not a named variant.

Rendered 13 time(s) in 12 other file(s).

#### FeatureShowcase (`apps/landing/src/components/FeatureShowcase.tsx`:31)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `tints` | `lavender` | `bg-[#f3edf9]` | 0 |
| `tints` | `peach` | `bg-[#fcf2e9]` | 0 |
| `tints` | `mint` | `bg-[#edf7ef]` | 0 |
| `tints` | `sky` | `bg-[#eef2fb]` | 0 |

Rendered 5 time(s) in 1 other file(s).

#### BookmarkTagsEditor (`apps/web/components/dashboard/bookmarks/BookmarkTagsEditor.tsx`:10)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `field` | _declared by the prop type only_ | 0 |
| `variant` | `inline` | _declared by the prop type only_ | 3 |

Rendered 4 time(s) in 4 other file(s).

#### InfoTooltip (`apps/web/components/ui/info-tooltip.tsx`:10)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `tip` | _declared by the prop type only_ | 0 |
| `variant` | `explain` | _declared by the prop type only_ | 2 |

Rendered 4 time(s) in 4 other file(s).

#### BookmarkTextMarkdown (`apps/mobile/components/bookmarks/BookmarkTextMarkdown.tsx`:5)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `size` | `body` | _declared by the prop type only_ | 0 |
| `size` | `subhead` | _declared by the prop type only_ | 2 |

1 conditional class branch(es) in this file are not a named variant.

Rendered 3 time(s) in 3 other file(s).

#### ListPicker (`apps/mobile/components/lists/list-picker.tsx`:48)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `state` | `selected` | _declared by the prop type only_ | 0 |
| `state` | `loading` | _declared by the prop type only_ | 0 |

States targeted in this file: `active`, `disabled`

Rendered 3 time(s) in 3 other file(s).

#### TagsEditor (`apps/web/components/dashboard/bookmarks/TagsEditor.tsx`:35)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `field` | _declared by the prop type only_ | 0 |
| `variant` | `inline` | _declared by the prop type only_ | 1 |
| `attachedBy` | `human` | _declared by the prop type only_ | 0 |
| `attachedBy` | `ai` | _declared by the prop type only_ | 0 |

States targeted in this file: `after`, `dark`, `focus`, `focus-visible`, `focus-within`, `has-[>svg]`, `hover`, `placeholder`

2 conditional class branch(es) in this file are not a named variant.

Rendered 3 time(s) in 3 other file(s).

#### Toggle (`apps/web/components/ui/toggle.tsx`:32)

Always applied: `inline-flex items-center justify-center rounded-md text-sm font-medium transition-colors hover:bg-muted hover:text-muted-foreground focus-visible:outline-none focus-visible:ring-[3px] focus-visible:ring-ring/50 disabled:pointer-events-none disabled:opacity-50 data-[state=on]:bg-accent data-[state=on]:text-accent-foreground`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `default` _(default)_ | `bg-transparent` | 0 |
| `variant` | `outline` | `border border-input bg-transparent hover:bg-accent hover:text-accent-foreground` | 2 |
| `size` | `default` _(default)_ | `h-10 px-3` | 0 |
| `size` | `sm` | `h-9 px-2.5` | 0 |
| `size` | `lg` | `h-11 px-5` | 0 |

States targeted in this file: `data-[state=on]`, `disabled`, `focus-visible`, `hover`

Rendered 3 time(s) in 3 other file(s).

#### DialogOverlay (`apps/web/components/ui/dialog.tsx`:17)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `size` | `sm` | _declared by the prop type only_ | 0 |
| `size` | `lg` | _declared by the prop type only_ | 0 |

States targeted in this file: `data-[state=closed]`, `data-[state=open]`, `disabled`, `focus-visible`, `has-[[data-dialog-body]]`, `hover`

1 conditional class branch(es) in this file are not a named variant.

Rendered 2 time(s) in 2 other file(s).

#### ReaderSettingsPopover (`apps/web/components/dashboard/preview/ReaderSettingsPopover.tsx`:66)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `outline` | _declared by the prop type only_ | 0 |
| `variant` | `ghost` | _declared by the prop type only_ | 1 |

States targeted in this file: `after`, `dark`, `hover`

1 conditional class branch(es) in this file are not a named variant.

Rendered 2 time(s) in 2 other file(s).

#### ThemeProvider (`apps/browser-extension/src/utils/ThemeProvider.tsx`:24)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `currentTheme` | `light` | _declared by the prop type only_ | 0 |
| `currentTheme` | `dark` | _declared by the prop type only_ | 0 |

Rendered 2 time(s) in 2 other file(s).

#### Toaster (`apps/web/components/ui/sonner.tsx`:16)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `destructive` | _declared by the prop type only_ | 0 |
| `variant` | `default` | _declared by the prop type only_ | 0 |

States targeted in this file: `dark`, `group-[.toast]`, `group-[.toaster]`

Rendered 2 time(s) in 2 other file(s).

#### AdminNotices (`apps/web/components/admin/AdminNotices.tsx`:29)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `level` | `info` | _declared by the prop type only_ | 0 |
| `level` | `warning` | _declared by the prop type only_ | 0 |
| `level` | `error` | _declared by the prop type only_ | 0 |

Rendered 1 time(s) in 1 other file(s).

#### BookmarkDebugger (`apps/web/components/admin/BookmarkDebugger.tsx`:42)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `status` | `pending` | _declared by the prop type only_ | 0 |
| `status` | `failure` | _declared by the prop type only_ | 0 |
| `status` | `success` | _declared by the prop type only_ | 0 |

States targeted in this file: `hover`

Rendered 1 time(s) in 1 other file(s).

#### DropdownMenuSubTrigger (`apps/web/components/ui/dropdown-menu.tsx`:21)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `default` | _declared by the prop type only_ | 0 |
| `variant` | `destructive` | _declared by the prop type only_ | 0 |

States targeted in this file: `dark`, `data-[disabled]`, `data-[side=bottom]`, `data-[side=left]`, `data-[side=right]`, `data-[side=top]`, `data-[state=closed]`, `data-[state=open]`, `data-[variant=destructive]`, `focus`

Rendered 1 time(s) in 1 other file(s).

#### Field (`apps/web/components/ui/field.tsx`:85)

Always applied: `group/field flex w-full gap-3 data-[invalid=true]:text-destructive`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `orientation` | `vertical` _(default)_ | `["flex-col [&>*]:w-full [&>.sr-only]:w-auto"]` | 0 |
| `orientation` | `horizontal` | `[ "flex-row items-center", "[&>[data-slot=field-label]]:flex-auto", "has-[>[data-slot=field-content]]:[&>[role=checkbox],[role=radio]]:mt-px has-[>[data-slot=field-content]]:items-start", ]` | 1 |
| `orientation` | `responsive` | `[ "@md/field-group:flex-row @md/field-group:items-center @md/field-group:[&>*]:w-auto flex-col [&>*]:w-full [&>.sr-only]:w-auto", "@md/field-group:[&>[data-slot=field-label]]:flex-auto", "@md/field-group:has-[>[data-slot=field-content]]:items-start @md/field-group:has-[>[data-slot=field-content]]:[&>[role=checkbox],[role=radio]]:mt-px", ]` | 0 |

States targeted in this file: `dark`, `data-[invalid=true]`, `data-[slot=checkbox-group]`, `data-[variant=label]`, `data-[variant=legend]`, "group-data-[disabled=true]/field", "group-data-[variant=outline]/field-group", "group-has-[[data-orientation=horizontal]]/field", `has-[>[data-slot=checkbox-group]]`, `has-[>[data-slot=field-content]]`, `has-[>[data-slot=field]]`, `has-[>[data-slot=radio-group]]`, `has-data-[state=checked]`, `last`

Rendered 1 time(s) in 1 other file(s).

#### InvitationRow (`apps/mobile/components/lists/pending-list-invitations.tsx`:18)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `role` | `viewer` | _declared by the prop type only_ | 0 |
| `role` | `editor` | _declared by the prop type only_ | 0 |

Rendered 1 time(s) in 1 other file(s).

#### ReadingSettings (`apps/web/components/settings/ReadingSettings.tsx`:36)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `key` | `fontSize` | _declared by the prop type only_ | 0 |
| `key` | `lineHeight` | _declared by the prop type only_ | 0 |
| `key` | `fontFamily` | _declared by the prop type only_ | 0 |

Rendered 1 time(s) in 1 other file(s).

#### SubscriptionSettings (`apps/web/components/settings/SubscriptionSettings.tsx`:19)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `status` | `free` | _declared by the prop type only_ | 0 |
| `status` | `custom` | _declared by the prop type only_ | 0 |
| `status` | `paid` | _declared by the prop type only_ | 0 |

States targeted in this file: `active`, `dark`, `hover`

2 conditional class branch(es) in this file are not a named variant.

Rendered 1 time(s) in 1 other file(s).

#### UpdateUserDialog (`apps/web/components/admin/UpdateUserDialog.tsx`:51)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `currentRole` | `user` | _declared by the prop type only_ | 0 |
| `currentRole` | `admin` | _declared by the prop type only_ | 0 |

States targeted in this file: `open`

Rendered 1 time(s) in 1 other file(s).

#### ViewOptions (`apps/web/components/dashboard/ViewOptions.tsx`:66)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `fit` | `cover` | _declared by the prop type only_ | 0 |
| `fit` | `contain` | _declared by the prop type only_ | 0 |

Rendered 1 time(s) in 1 other file(s).

#### ActionToast (`apps/mobile/components/ui/Toast.tsx`:56)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `toast` | `default` | `bg-foreground` | 0 |
| `toast` | `destructive` | `bg-destructive` | 0 |
| `toast` | `success` | `bg-green-500` | 0 |
| `toast` | `info` | `bg-blue-500` | 0 |
| `position` | `top` | _declared by the prop type only_ | 0 |
| `position` | `bottom` | _declared by the prop type only_ | 0 |

States targeted in this file: `dark`

Rendered 0 time(s) in 0 other file(s).

#### BookmarkDefaultViewSettings (`apps/mobile/app/dashboard/settings/bookmark-default-view.tsx`:14)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `mode` | `reader` | _declared by the prop type only_ | 0 |
| `mode` | `browser` | _declared by the prop type only_ | 0 |
| `mode` | `externalBrowser` | _declared by the prop type only_ | 0 |

Rendered 0 time(s) in 0 other file(s).

#### BookmarkFooterMetadata (`apps/mobile/components/bookmarks/BookmarkCard.tsx`:51)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `align` | `start` | _declared by the prop type only_ | 0 |
| `align` | `end` | _declared by the prop type only_ | 0 |

States targeted in this file: `dark`

1 conditional class branch(es) in this file are not a named variant.

Rendered 0 time(s) in 0 other file(s).

#### Divider (`apps/mobile/components/ui/Divider.tsx`:5)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `orientation` | `horizontal` | _declared by the prop type only_ | 0 |
| `orientation` | `vertical` | _declared by the prop type only_ | 0 |

States targeted in this file: `dark`

1 conditional class branch(es) in this file are not a named variant.

Rendered 0 time(s) in 0 other file(s).

#### FieldSet (`apps/web/components/ui/field.tsx`:11)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `legend` | _declared by the prop type only_ | 0 |
| `variant` | `label` | _declared by the prop type only_ | 0 |

States targeted in this file: `dark`, `data-[invalid=true]`, `data-[slot=checkbox-group]`, `data-[variant=label]`, `data-[variant=legend]`, "group-data-[disabled=true]/field", "group-data-[variant=outline]/field-group", "group-has-[[data-orientation=horizontal]]/field", `has-[>[data-slot=checkbox-group]]`, `has-[>[data-slot=field-content]]`, `has-[>[data-slot=field]]`, `has-[>[data-slot=radio-group]]`, `has-data-[state=checked]`, `last`

Rendered 0 time(s) in 0 other file(s).

#### IssueBadge (`apps/web/app/settings/broken-links/page.tsx`:91)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `issue` | `blocked` | `bg-amber-500/10 text-amber-700 dark:text-amber-400` | 0 |
| `issue` | `missing` | `bg-rose-500/10 text-rose-700 dark:text-rose-400` | 0 |
| `issue` | `server` | `bg-orange-500/10 text-orange-700 dark:text-orange-400` | 0 |
| `issue` | `failed` | `bg-muted text-muted-foreground` | 0 |
| `issue` | `http` | `bg-muted text-muted-foreground` | 0 |
| `action` | `retry` | _declared by the prop type only_ | 0 |
| `action` | `delete` | _declared by the prop type only_ | 0 |

States targeted in this file: `dark`, `disabled`, `hover`

Rendered 0 time(s) in 0 other file(s).

#### TagPickerPage (`apps/mobile/app/dashboard/bookmarks/[slug]/manage_tags.tsx`:25)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `action` | `attach` | _declared by the prop type only_ | 0 |
| `action` | `detach` | _declared by the prop type only_ | 0 |

States targeted in this file: `active`, `checked`, `placeholder`

Rendered 0 time(s) in 0 other file(s).

#### TagRow (`apps/web/components/dashboard/bookmarks/BulkTagModal.tsx`:29)

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `action` | `add` | _declared by the prop type only_ | 0 |
| `action` | `remove` | _declared by the prop type only_ | 0 |

States targeted in this file: `focus-visible`, `hover`, `open`

Rendered 0 time(s) in 0 other file(s).

#### Toast (`apps/web/components/ui/toast.tsx`:43)

Always applied: `group pointer-events-auto relative flex w-full items-center justify-between space-x-4 overflow-hidden rounded-md border p-6 pr-8 shadow-lg transition-all data-[swipe=cancel]:translate-x-0 data-[swipe=end]:translate-x-[var(--radix-toast-swipe-end-x)] data-[swipe=move]:translate-x-[var(--radix-toast-swipe-move-x)] data-[swipe=move]:transition-none data-[state=open]:animate-in data-[state=closed]:animate-out data-[swipe=end]:animate-out data-[state=closed]:fade-out-80 data-[state=closed]:slide-out-to-right-full data-[state=open]:slide-in-from-top-full data-[state=open]:sm:slide-in-from-bottom-full`

| axis | value | classes | call sites |
| --- | --- | --- | --- |
| `variant` | `default` _(default)_ | `border bg-background text-foreground` | 0 |
| `variant` | `destructive` | `destructive group border-destructive bg-destructive text-destructive-foreground` | 0 |

States targeted in this file: `data-[state=closed]`, `data-[state=open]`, `data-[swipe=cancel]`, `data-[swipe=end]`, `data-[swipe=move]`, `disabled`, `focus`, `focus-visible`, `group-[.destructive]`, `group-hover`, `hover`

Rendered 0 time(s) in 0 other file(s).
