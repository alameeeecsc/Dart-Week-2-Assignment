double calculateTotal(List<double> prices, {double taxRate = 0}) {
  double subtotal = prices.reduce((a, b) => a + b);
  return subtotal + (subtotal * taxRate);
}
