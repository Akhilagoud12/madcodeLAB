# madcodeLAB
#calulator java code
package com.example.caluclator;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.view.View;
import android.widget.EditText;

public class MainActivity extends AppCompatActivity {
    EditText et1, et2;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }

    public void add(View view) {
        et1 = (EditText) findViewById(R.id.editTextText);
        et2 = (EditText) findViewById(R.id.editTextText2);
        int a = Integer.parseInt(et1.getText().toString());
        int b = Integer.parseInt(et1.getText().toString());
        int c = a + b;
        EditText et3 = (EditText) findViewById(R.id.editTextText3);
        et3.setText("Addition" + c);
    }
