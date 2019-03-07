```actionscript
func isTestFlight() -> Bool {
  guard let appStoreReceiptURL = Bundle.main.appStoreReceiptURL else {
    return false
  }
  return appStoreReceiptURL.lastPathComponent == "sandboxReceipt"
}
```