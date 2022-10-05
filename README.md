# quackifier
I tried following a tutorial and completely failed LOL
import SwiftUI

struct ContentView: View {
    @State var text = ""
    @State var title = "Hello human"
    var body: some View {
        VStack {
            Image(systemName: 
                    "smiley.fill")
                .imageScale(.large)
                .foregroundColor(.accentColor)
                .padding(.top, 50)
            Text(title)
                .font(.largeTitle)
            
            Spacer()
            TextField("Enter something", text: $text)
                .multilineTextAlignment(.center)
                    .frame(width: 300)
            
            
            Spacer()
            
            Button("Submit") {
                
            }
            
            Spacer()
        }
        .padding()
        .frame(maxWidth: .infinity, maxHeight: .infinity)
        .background(Color(red: 0.024, green: 0.392, blue: 0.0549))
        .ignoresSafeArea()
    }
}
